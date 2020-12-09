# Templates for Haskell Projects

This project uses [stack-templates](https://github.com/commercialhaskell/stack-templates) to create a haskell project from a description.

## Templates

- [cabal-stack](./cabal-stack.hsfiles): cabal + stack
- [cabal-stack-ci](./cabal-stack-nix-ci.hsfiles): cabal + stack + travisCI + githubActions
- [cabal-stack-nix-ci](./cabal-stack-nix-ci.hsfiles): cabal + stack + nix + travisCI + githubActions

## How-to

In order to create a new project from this template:

```bash
git clone git@github.com:monadplus/haskell-templates.git

stack new <project-name> <template-name> -p "synopsis:???" -p "description:???" -p "category:???"
```
