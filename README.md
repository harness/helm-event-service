# event-service

![Version: 0.1.3](https://img.shields.io/badge/Version-0.1.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.773.0](https://img.shields.io/badge/AppVersion-1.773.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `true` |  |
| autoscaling.maxReplicas | int | `2` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| ce-gcp-home-project-creds | string | `""` |  |
| defaultInternalImageConnector | string | `"test"` |  |
| eventSvcServiceAccounts.ceGCPHomeProjectCreds.key | string | `"placeHolderKey"` |  |
| eventSvcServiceAccounts.ceGCPHomeProjectCreds.name | string | `"placeHolderName"` |  |
| fullnameOverride | string | `""` |  |
| global.ingress.className | string | `"harness"` |  |
| global.ingress.enabled | bool | `false` |  |
| global.ingress.hosts[0] | string | `"events-grpc-app.harness.io"` |  |
| global.ingress.tls.enabled | bool | `true` |  |
| global.ingress.tls.secretName | string | `""` |  |
| global.loadbalancerURL | string | `"https://test"` |  |
| image.digest | string | `""` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"harness/event-service-signed"` |  |
| image.tag | string | `"77317"` |  |
| ingress.className | string | `"nginx"` |  |
| java.memory | int | `1024` |  |
| maxSurge | string | `"100%"` |  |
| maxUnavailable | int | `0` |  |
| mongoSecrets.password.key | string | `"mongodb-root-password"` |  |
| mongoSecrets.password.name | string | `"mongodb-replicaset-chart"` |  |
| mongoSecrets.userName.key | string | `"mongodbUsername"` |  |
| mongoSecrets.userName.name | string | `"harness-secrets"` |  |
| nameOverride | string | `""` |  |
| ngServiceAccount | string | `"test"` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| redislabsCATruststore | string | `"test"` |  |
| replicaCount | int | `2` |  |
| resources.limits.cpu | string | `"512m"` |  |
| resources.limits.memory | string | `"1440Mi"` |  |
| resources.requests.cpu | string | `"512m"` |  |
| resources.requests.memory | string | `"1440Mi"` |  |
| securityContext | object | `{}` |  |
| service.port | int | `7280` |  |
| service.port2 | int | `9889` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| timescaleSecret.password.key | string | `"timescaledbPostgresPassword"` |  |
| timescaleSecret.password.name | string | `"harness-secrets"` |  |
| tolerations | list | `[]` |  |
| waitForInitContainer.image.digest | string | `""` |  |
| waitForInitContainer.image.pullPolicy | string | `"IfNotPresent"` |  |
| waitForInitContainer.image.registry | string | `"docker.io"` |  |
| waitForInitContainer.image.repository | string | `"harness/helm-init-container"` |  |
| waitForInitContainer.image.tag | string | `"latest"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
