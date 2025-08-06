## Helm Chart

```shell
helm repo add wonkyooh https://wonkyooh.github.io/helm-charts
```

```shell
helm repo update wonkyooh
```

```shell
helm search repo wonkyooh
```

## Register a chart

Get the compressed chart from the repository or chart directory of your choice.

```shell
helm pull <repo>/<chart> --version <version>
```

```shell
helm pull <chart> --repo <repoURL> --version <version>
```

```shell
helm pull <chartURL> --version <version>
```

```shell
helm package <chartDir>
```

Move the compressed chart to the `charts` directory.

```shell
mv <chart>-<version>.tgz ./charts
```

Update the `index.yaml` file.

```shell
make index
```
