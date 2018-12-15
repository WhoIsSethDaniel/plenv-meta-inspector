# NAME

plenv-meta-inspector - subcommands for plenv that provide inspection of modules and their details

# SYNOPSIS

      # list all core modules and their versions for the current Perl
      plenv list-core-modules

      # list all CPAN installed modules and their versions for the current Perl
      plenv list-cpan-modules

      # list all files installed by the given distribution/s. (by default
      # the listed files are relative to the current Perl's directory.)
      plenv list-files Moo 

      # list absolute paths to files installed by the given distribution/s
      plenv list-files -f Moo

# DESCRIPTION

Adds several new sub-commands to plenv that help with inspecting details of
the modules that are installed in your current plenv environment.

# COMMANDS

### plenv list-core-modules

List all the core modules for the currently selected Perl as well the version
of each module.

### plenv list-cpan-modules

Similar to the `list-modules` subcommand, but lists all the CPAN installed
modules for the currently selected Perl as well as the version of each module.  

### plenv list-files

List all installed files for the given list of distributions.  

# INSTALLATION

First, install [plenv](https://github.com/tokuhirom/plenv) if you have not 
already done so.

Second, checkout plenv-meta-inspector into your `~/.plenv/plugins`.

  ```sh
  $ git clone https://github.com/whoissethdaniel/plenv-meta-inspector ~/.plenv/plugins/meta-inspector
  ```

That's it!
