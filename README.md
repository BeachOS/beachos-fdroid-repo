F-Droid repo for various apps
========================================

Currently included (alphabetically):

* 

Not meant to be added to F-Droid manually, this is shipped with BeachOS

Both, this Gitlab repository and this unofficial F-Droid repository
are not affiliated to, nor have been authorized, sponsored or otherwise approved by the app developers.

This is based on https://gitlab.com/rfc2822/fdroid-firefox


How does it work?
=================

This unofficial F-Droid repository is hosted using [Gitlab pages](https://about.gitlab.com/2016/04/07/gitlab-pages-setup/).
A daily [scheduled pipeline](https://docs.gitlab.com/ce/user/project/pipelines/schedules.html)
downloads the APKs either dirctly from the app developers, or from F-Droid repos and then updates this F-Droid repository, which is then shipped with the OS.<br />
All necessary actions are performed by [Gitlab CI/CD](https://about.gitlab.com/features/gitlab-ci-cd/).
This Gitlab repository contains the complete source code to configure Gitlab CI/CD and this F-Droid repository.

The private key for signing this F-Droid repository is kept private, but only used for exactly this purpose.<br />
The APKs are unaltered and hence still signed by the app developers.
