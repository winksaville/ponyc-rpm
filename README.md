# Install ponyc from .rpm files
This installs ponyc using `makepkg -si` from the release .rpm
files on [bintray](https://bintray.com/pony-language/ponyc-rpm)

The current ponyc package installed via pacman is not compatible with
LLVM5 and fails, see Arch Linux bug
[55170](https://bugs.archlinux.org/task/55170) archlinux bug.
It is also not possible to build ponyc from source for
the same reason.

[Issue 2303](https://github.com/ponylang/ponyc/pull/2303)
is tracking the problem.

This was based on a guide from
[nemrod](http://nemrod.se/guides/install-rpm-packages-on-arch-linux)
and in particular the
[comment from Hi-Angel](http://nemrod.se/guides/install-rpm-packages-on-arch-linux/#comment-183470)
in January 2017.
