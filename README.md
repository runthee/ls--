# NAME

ls++ - colorized ls on steroids

# USAGE

ls++ \[OPTION\]... \[FILE\]...

# DESCRIPTION

### GNU/Linux

  ![GNU/Linux screenshot](http://devel.japh.se/App::ls++/ls++_xterm.png)

### MacOSX / *BSD

  Please provide a screenshot, Mac users.

### GNU/Linux TTY/VC

  TODO

# OPTIONS

Not known parameters will be passed through to **ls**, so to show hidden files,
**-a** or **-A** might be added. See **ls(1)** for more information.

### Views

    --pf    permissions, file
    --psf   permissions, size, file
    --tpf   time, permissions, file
    --tpsf  time, permissions, size, file (default)
    --ptsf  permissions, time, size, file

# INSTALLATION

    cpan Term::ExtendedColor
    git clone git://github.com/trapd00r/ls--.git
    cd ls--
    perl Makefile.PL
    make && su -c 'make install'

    cp ls++.conf $HOME/.ls++.conf

# HISTORY

I wanted to re-arrange the ls output just like one can do with the -printf
option to GNU find. Sadly, there are no -printf option available for ls, so I
threw together a quick hack called 'pilsner' that did what I wanted and nothing
more, nothing less. Not very useful to others.

Mattias Svanström crafted together the 'l' application which did basicly the
same thing but more elegant and with a nice twist; it calculated relative
mtimes.

I really liked that idea, but there were a couple of annoyances, so I forked the
project and added a configuration file, support for flags that'll control the
different views and possiblity to ignore as well as highlight specific files.

# AUTHOR

    \ \ | / /
     \ \ - /
      \ | /
      (O O)
      ( < )
      (-=-)

    Magnus Woldrich
    CPAN ID: WOLDRICH
    m@japh.se
    http://japh.se

# CONTRIBUTORS

[Mattias Svanström][0]

[Gregory Sacre][1]


# COPYRIGHT

Copyright 2010, 2011 the **ls++** AUTHOR and CONTRIBUTORS as listed above.

# SEE ALSO

[l][2]

[pilsner][3]

[0]: http://github.com/mmso
[1]: https://github.com/gsacre
[2]: http://github.com/mmso/scripts
[3]: http://github.com/trapd00r/utils/blob/master/pilsner
