# Traefik

Ingress controller with focus on simplicity.

## Getting started

```
# Fetch package
kpt pkg get https://github.com/WitoDelnat/katalog/traefik traefik

# Deploy package
kustomize build traefik | k apply -f -
```

## Configuration

**Last-mile configuration**

You can configure some commonly set values through setters.

```
# See available setters
kpt cfg list-setters traefik

# Change value of setter
kpt cfg set . $setterName $setterValue
```

**Advanced configuration**

You can modify the files as you would with any Kustomize file.
[Kpt update][kpt-update] shows how these modifications can be dealt with in updates.

[pilot]: https://traefik.io/traefik-pilot/
[kpt-update]: https://googlecontainertools.github.io/kpt/reference/pkg/update/
