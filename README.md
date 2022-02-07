# Legacy Package Sets

A curated set of PureScript packages known to compile together, for `psc-package` and `spago`.

This repository is a mirror of the package sets produced by the [PureScript Registry](https://github.com/purescript/registry), in a legacy format intended to support `psc-package` and `spago` users who are not using the registry.

## For Developers

This repository used to manage package sets for `psc-package` and `spago` users. With the launch of the [PureScript Registry](https://github.com/purescript/registry), which produces package sets automatically, this repository has become a legacy mirror only.

When a new package set is produced by the `registry`, a few things happen:

1. The registry transforms the package set into the legacy format.
2. The registry CI adds the legacy format `packages.dhall` and `packages.json` files to this repository.
3. The registry CI updates the `latest-compatible-sets` file in this repository.
4. The registry CI commits the changes and pushes a new tag, `psc-compiler-date`, to this repository.
5. The package sets CI (this repository) produces a new release using the new package sets files.

For this reason, this repository only contains the package set files, the compatible sets file, and the CI necessary to trigger new releases when a tag is added to the repository.
