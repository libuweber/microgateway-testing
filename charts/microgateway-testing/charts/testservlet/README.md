testservlet
===========
TestServlet for Web Application firewall (WAF).

Current chart version is `1.0`

Source code can be found [here](https://www.airlock.com)



## Chart Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| exposedport | int | `8080` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"julianbe/microgateway"` |  |
| image.tag | string | `"testservlet-1.13"` |  |
| imagePullSecrets | list | `[]` |  |
| livenessProbe.failureThreshold | int | `3` |  |
| livenessProbe.initialDelaySeconds | int | `10` |  |
| livenessProbe.path | string | `"/TestServlet/"` |  |
| livenessProbe.periodSeconds | int | `5` |  |
| livenessProbe.scheme | string | `"HTTP"` |  |
| livenessProbe.successThreshold | int | `1` |  |
| livenessProbe.timeoutSeconds | int | `4` |  |
| port | int | `8080` |  |
| protocol | string | `"TCP"` |  |
| readinessProbe.failureThreshold | int | `3` |  |
| readinessProbe.initialDelaySeconds | int | `5` |  |
| readinessProbe.path | string | `"/TestServlet/"` |  |
| readinessProbe.periodSeconds | int | `5` |  |
| readinessProbe.scheme | string | `"HTTP"` |  |
| readinessProbe.successThreshold | int | `1` |  |
| readinessProbe.timeoutSeconds | int | `4` |  |
