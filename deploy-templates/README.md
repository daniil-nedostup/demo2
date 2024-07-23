# echo-server

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

A Helm chart for Kubernetes

**Homepage:** <https://github.com/daniil-nedostup/echo-server>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| KubeRocketCI |  | <https://github.com/epam/edp-install/> |

## Source Code

* <https://github.com/daniil-nedostup/echo-server>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| application.enable.cookies | bool | `true` | Enable cookies in response |
| application.enable.environment | bool | `true` | Enable environment in response |
| application.enable.file | bool | `true` | Enable file in response |
| application.enable.header | bool | `true` | Enable custom header in response |
| application.enable.host | bool | `true` | Enable host in response |
| application.enable.http | bool | `true` | Enable http in response |
| application.enable.request | bool | `true` | Enable request in response |
| application.logs.ignore.ping | bool | `false` | Don't log ping request on route `/ping` |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repo | string | `"ealen/echo-server"` |  |
| image.version | string | `"0.9.2"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"cluster.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| livenessProbe.failureThreshold | int | `3` |  |
| livenessProbe.httpGet.httpHeaders[0].name | string | `"x-echo-code"` |  |
| livenessProbe.httpGet.httpHeaders[0].value | string | `"200"` |  |
| livenessProbe.httpGet.path | string | `"/ping"` |  |
| livenessProbe.initialDelaySeconds | int | `5` |  |
| livenessProbe.periodSeconds | int | `10` |  |
| livenessProbe.successThreshold | int | `1` |  |
| livenessProbe.timeoutSeconds | int | `2` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"50m"` |  |
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"50m"` |  |
| resources.requests.memory | string | `"128Mi"` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

