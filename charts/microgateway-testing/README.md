Airlock microgateway-testing
====================

Testing chart for Web Application firewall (WAF).

:warning: **For internal testing purposes only.**:

## Adding the Repository

To add the chart repository:

```console
helm repo add airlock-testing https://libuweber.github.io/microgateway-testing/
```

## Installing the Chart

To install the chart with the release name `airlock-testing`:

```console
helm upgrade -i airlock-testing airlock/microgateway-testing
```

## Uninstalling the Chart

To uninstall the chart with the release name `airlock-testing`:

```console
helm uninstall airlock-testing
```

## Configuration

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| echo-server.enabled | bool | `false` |  |
| echo-server.fullnameOverride | string | `"backend-service"` |  |
| echo-server.service.port | int | `8080` |  |
| testservlet.enabled | bool | `true` |  |
| testservlet.fullnameOverride | string | `"testservlet"` |  |

## Chart dependencies
The helm chart has optional dependencies which can be activated.

| Repository | Name | Version |
|------------|------|---------|
|  | testservlet | 1.0 |
| https://ealenn.github.io/charts | echo-server | 0.3.0 |
| https://libuweber.github.io/microgateway | microgateway | 0.3.4 |