# Templates for Haskell

## Simple

This template includes a project skeleton integrated with:
- Cabal
- Stack
- Nix
- CI: Github Actions

```bash
stack new <project-name> github:monadplus/basic
```

### Set up

Github Actions require to set the `CACHIX_AUTH_TOKEN` for the `nix` step:
1. Create a [Cachix](https://app.cachix.org/) account, 'Create a binary cache' (or use an existing one), go to the binary cache 'Settings', create a new 'Cache Auth Tokens' with read/write permissions and store it on your local machine.
2. Go to https://github.com/{username}/{project}/settings/secrets/actions (replace `{username}` and `{project}`).
3. Create a new secret called `CACHIX_AUTH_TOKEN` and set its value to the token generated on step (1).
