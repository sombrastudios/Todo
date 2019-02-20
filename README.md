# Todo

Simple CLI Tool to note down TODOs (W.I.P and not yet ready)


_Note: the following is just a showcase of planned usage of `todo`_
### In order to create new TODOs write the following
```sh
    #   Will create a new TODO in list `Linear Algebra`
    #   if --list is not specified, it will simply use the general list called "" (Empty String)
    $ todo new --list="Linear Algebra" "Research Change of Basis"

    #   This way a prompt will be spawned
    $ todo new
    >   Category:
            USER INPUT
    >   Description:
            USER INPUT
```

### To show your TODOs type this
```sh
    # Show unfinished TODOs in all lists
    $ todo show

    # Show _all_ TODOs
    $ todo show -a

    # Show unfinished TODOs in list `Linear Algebra`
    $ todo show "Linear Algebra"

    # Show _all_ TODOs in list `Linear Algebra`
    $ todo show -a "Linear Algebra"
    # or
    $ todo show "Linear Algebra" -a
```

### Manage your TODOs
```sh
    # ID stands for avariable lenght list of IDs generated by the program _on runtime_
    $ todo set ...<id> done
    $ todo set ...<id> undone

    # Remove TODOs permanently
    $ todo remove ...<id>
    # Remove all TODOs permanently
    $ todo remove --all
```

### Show all available lists
```sh
    $ todo list
    # If you want to see how many TODOs are left to do and how many are done, pass the `ratio` flag
    $ todo list -r
    $ todo list --ratio
```
