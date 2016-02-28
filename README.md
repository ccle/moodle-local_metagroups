# Meta-course group synchronization [![Build Status](https://travis-ci.org/paulholden/moodle-local_metagroups.svg?branch=master)](https://travis-ci.org/paulholden/moodle-local_metagroups)

## Requirements

- Moodle 3.5.3 or later.
- Meta-course enrolment plugin.

## Installation

Copy the metagroups folder into your Moodle /local directory and visit your admin notification page to complete the installation.

## Usage

After installation, or when creating new meta-course enrolment instances, you may need to synchronize existing groups. To do this
run the cli/sync.php script (use the --help switch for further instructions on usage) or enable Meta-course group synchronization
scheduled task.

Any future amendments to groups (add, update and delete) and their membership (add or remove users) in 'child' courses will be automatically
reflected in 'parent' courses that use groups.

## Author

Paul Holden (pholden@greenhead.ac.uk)
Vadim Dvorovenko (Vadimon@mail.ru)

- Updates: https://moodle.org/plugins/view.php?plugin=local_metagroups
- Latest code: https://github.com/paulholden/moodle-local_metagroups

Changes
-------
Release 1.4.0 (build 2016022800):
- Add scheduled tasks for synchronization.

Release 1.3 (build 2014103100):
- CLI script can now synchronize specific courses.
- API & documentation updates.

Release 1.2 (build 2014080500):
- Only synchronize parent courses that use groups.

Release 1.1 (build 2014031300):
- Prevent synchronized group memberships being removed.

Release 1.0 (build 2014021001):
- First release.
