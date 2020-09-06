# Katalog

A kubernetes catalog of kpt packages.

## Usage

1. Fetch

```
kpt pkg get https://github.com/WitoDelnat/katalog/$PKG_NAME
```

2. Add last-mile configurations

```
kpg cfg list-setters .
```

> The `/instance` directory can contain additional configuration files. For example, `prometheus.yml` or application environment variables.

> The `/instance` directory is where you can add patches for when the out-of-the-box configuration is not sufficient.

3. Deploy

```
kustomize build . | kubectl apply -f -
```
