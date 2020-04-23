# Medusa plugins

This is just an idea to see if I can create a generic plugin system for `cobra`


## references

There is some previous work, but all too specific to one command.

- krew for kubectl
- git plugins
- buffalo plugins


## general idea

All follow a similar pattern:

- compose the subcomand name
- search the binary in $PATH 
- execute it

A helper package can help leverage all this boilerplate code and make it simple to discover, add and run plugins.


## features to consider

- multi language support (go, bash, etc)
- discover and install plugins easily like scoop or brew
- sub command should be aware of environment and parent flags

