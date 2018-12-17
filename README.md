# NAME

plenv-module-inspector - subcommands for plenv that provide inspection of modules and their details

# SYNOPSIS

      # list all core modules and their versions for the current Perl
      plenv list-core-modules

      # list all CPAN installed distributions and their versions for the 
      # current Perl
      plenv list-dists

      # list all CPAN installed modules and their versions
      plenv list-cpan-modules

      # list all CPAN installed modules, their versions, their distribution,
      # and the relative path to the file
      plenv list-cpan-modules -a

      # list all files installed by the given distribution/s. (by default
      # the listed files are relative to the current Perl's directory.)
      plenv list-files Moo 

      # list absolute paths to files installed by the given distribution/s
      plenv list-files -f Moo

# DESCRIPTION

Adds several new subcommands to plenv that help with inspecting details of
the modules that are installed in your current plenv environment.

# COMMANDS

### plenv list-core-modules

List all the core modules for the currently selected Perl as well the version
of each module.

### plenv list-dists

Similar to the `list-modules` subcommand, but lists all the CPAN installed
distributions for the currently selected Perl as well as the version of each 
distribution.

### plenv list-cpan-modules

List all CPAN installed modules plus their versions.  

### plenv list-files

List all installed files for the given list of distributions.  

# INSTALLATION

First, install [plenv](https://github.com/tokuhirom/plenv) if you have not 
already done so.

Second, checkout plenv-module-inspector into your `~/.plenv/plugins`.

  ```sh
  $ git clone https://github.com/whoissethdaniel/plenv-module-inspector ~/.plenv/plugins/module-inspector
  ```

That's it!

# BUG REPORTING

Use Github issues: https://github.com/WhoIsSethDaniel/plenv-module-inspector/issues

# AUTHOR

Seth Daniel <perl @ sethdaniel.org>

# SEE ALSO

[plenv](https://github.com/tokuhirom/plenv)

[ExtUtils::Installed](https://metacpan.org/pod/ExtUtils::Installed)

# LICENSE

None. Use it as you see fit.  

If you change it please consider submitting a patch.
