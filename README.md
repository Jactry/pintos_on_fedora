### Building Bochs

#### Install build dependencies

```
$ sudo dnf builddep bochs
$ sudo dnf groupinstall "C Development Tools and Libraries" "Development Tools"
```

#### Build Bochs

```
$ cd pintos_on_fedora/src/misc
# SRCDIR: folder contains bochs-2.2.6.tar.gz, PINTOSDIR: the root of the pintos source tree, DSTDIR: the installation prefix
$ SRCDIR="folder_where_you_put_bochs_source" PINTOSDIR="root_of_the_pintos_source_tree" DSTDIR=~/.local/opt/bochs ./bochs-2.2.6-build.sh
```

#### Add Bochs to $PATH

If you using bash as your shell, you can add this line to your .bashrc file:

`export PATH="$PATH:/home/your_username/.local/opt/bochs/bin"`

Or for zsh, you should add it in your .zshrc file.
