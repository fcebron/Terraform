# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
- [ ] Generates install list from a running system, then search in repositories if newest packages matches.
- [ ] Script "apt-mark showmanual" to generate a SoftwareList for installation migration.
- [ ] Specific installation of softwares which are not in the distribution's repositories.
- [ ] Adding config files for some specific packages like vim, ssh, redshift,...
- [ ] Add Debian support.
- [ ] Add Archlinux support.
- [ ] Add Fedora support.
- [ ] GUI for selecting softwares to install.
- [ ] Adding a parameter to skip the backport activation in "/etc/apt/sources.list.
- [ ] Add aptitude autoclean to clear the cache at the end.
- [ ] Add a "-s" option for a safe-upgrade instead of full-upgrade.
- [ ] Fix the ambiguous part of the reboot at the end of the program (currently it is a mix of 2 options => need to change it into one!)
- [ ] Turning the block of intructions to check if softwares are present, into a function (there is a redundancy).
- [ ] Test it under Ubuntu 18.04!
- [x] Adding ubuntu-restricted-addons to softwares lists.
- [x] Adding some parameters for the reboot options and to add an external software list.


## [[0.4.0](https://github.com/fcebron/Terraform/releases/tag/Terraform_0.4.0)] - 2018-05-02
### Added
- New name!
- Autoremove old dependencies.
- Asks for reboot at the end.


## [[0.3.0](https://github.com/fcebron/Terraform/releases/tag/Terraform_0.3.0)] - 2018-05-01
### Added
- Check before installation of removal if the software is already present on the system, to optimize the program.
- Check before exiting the program if all desired software have been installed.


## [[0.2.0](https://github.com/fcebron/Terraform/releases/tag/Terraform_0.2.0)] - 2018-05-01
### Added
- Test the internet connection with a ping to exit the program faster in case that there is no connection.
- Root check before executing full program.
- Parsing the .md file containing a list of software to install.
- Installation of the list of software.
- Suppression of selected pre-installed softwares before full-upgrade (to save some time, bandwidth,...).


## [[0.1.0](https://github.com/fcebron/Terraform/releases/tag/Terraform_0.1.0)] - 2018-04-28
### Added
- Automatic detection and installation (if missing) of Aptitude.
- Adding Canonical's partner repository to the system.
- Full Upgrade of the system.
- Coloured output of this script.
- Dated logfile of each installation.
- Tutorial explaining how to use this script.
