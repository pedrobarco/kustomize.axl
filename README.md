# kustomize.axl

Gazelle extension written in **AXL (Aspect Extension Language)** for generating and managing `BUILD.bazel` files for Kubernetes **Kustomize** configurations using `rules_kustomize`.

## Overview

`kustomize.axl` provides a Gazelle extension that:

- Detects `kustomization.yaml` files in a repository
- Generates corresponding `BUILD.bazel` targets
- Integrates with `rules_kustomize` for building Kustomize manifests with Bazel

The goal is to simplify maintaining Bazel targets for repositories that organize Kubernetes manifests using Kustomize.

## Development

Run Gazelle to update `BUILD.bazel` files:

```bash
bazel run //:gazelle
```

## References

- <https://github.com/aspect-build/aspect-gazelle>
- <https://github.com/seh/rules_kustomize>
