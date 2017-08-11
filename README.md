# git_checkout

This shows us a `git clone` vulnerability described in http://blog.recurity-labs.com/2017-08-10/scm-vulns

To see it in action, simply clone the repo using `git clone git@github.com:disconnect3d/git_clone_rce_calc.git --recursive` - the recursive part is crucial as git **must** try to clone the malicious git submodule url.

To be safe - upgrade to Git 2.14.1 as stated in [git's release notes](https://raw.githubusercontent.com/git/git/master/Documentation/RelNotes/2.14.1.txt).
