Main commands
=============

*info*
  Display information about current conda install.

*list*
  List linked packages in a conda environment.

*search*
  Search for packages and display their information. The input is a regular
  expression. To perform a search with a search string that starts with a -,
  separate the search from the options with --, like 'conda search -- -h'. A *
  in the results means that package is installed in the current environment. A
  . means that package is not installed but is cached in the pkgs directory.

*create*
  Create a new conda environment from a list of specified packages.

*install*
  Install a list of packages into a specified conda environment.

*update*
  Update conda packages to the current version.

*upgrade*
  Alias for conda update. See conda update --help.

*remove*
  Remove a list of packages from a specified conda environment.

*uninstall*
  Alias for conda remove. See conda remove --help.

*run*
  Launches an application installed with conda. To include command line options
  in a command, separate the command from the other options with --, like conda
  run -- ipython --matplotlib

*config*
  Modify configuration values in .condarc. This is modeled after the git config
  command. Writes to the user .condarc file (/Users/jdecock/.condarc) by
  default.

*init*
  Initialize conda into a regular environment (when conda was installed as a
  Python package, e.g. using pip). (DEPRECATED)

*clean*
  Remove unused packages and caches.

*package*
  Low-level conda package utility. (EXPERIMENTAL)

*bundle*
  Create or extract a "bundle package" (EXPERIMENTAL)

See also: http://conda.pydata.org/docs/_downloads/conda-cheatsheet.pdf


Update all installed packages
=============================

::

    conda update --all


Make virtual environments
=========================

::

    conda create -n cta python=3.4 anaconda
    source activate cta  # to switch to the cta python virtualenv

