# Overview

A (proof-of-concept level) script to store encrypted git credentials on a
per-shell basis. Requires python 3, pycrypto, bash, and linux or OSX.

# Usage

1. Put `git-credential-shell` in your path
2. Add to your bash login script of choice:
   `eval $(git-credential-shell setup)`
3. Configure git to use the script as a helper. Either:

   `git config --global credential.helper shell`

   to have it work for all your user's repositories, or

   `git config --local credential.helper shell`

   to install it only for the current repository.




