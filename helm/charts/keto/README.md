# keto

![Version: 0.19.3](https://img.shields.io/badge/Version-0.19.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.6.0](https://img.shields.io/badge/AppVersion-v0.6.0-informational?style=flat-square)

Access Control Policies as a Server

**Homepage:** <https://www.ory.sh/keto/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| ORY Team | hi@ory.sh | https://www.ory.sh/ |

## Source Code

* <https://github.com/ory/keto>
* <https://github.com/ory/k8s>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| automountServiceAccountToken | bool | `true` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| deployment.livenessProbe.failureThreshold | int | `5` |  |
| deployment.livenessProbe.initialDelaySeconds | int | `30` |  |
| deployment.livenessProbe.periodSeconds | int | `10` |  |
| deployment.readinessProbe.failureThreshold | int | `5` |  |
| deployment.readinessProbe.initialDelaySeconds | int | `30` |  |
| deployment.readinessProbe.periodSeconds | int | `10` |  |
| extraEnv | list | `[]` |  |
| extraVolumeMounts | list | `[]` |  |
| extraVolumes | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"oryd/keto"` |  |
| image.tag | string | `"v0.6.0-alpha.1-sqlite"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.read.annotations | object | `{}` |  |
| ingress.read.className | string | `""` |  |
| ingress.read.enabled | bool | `false` |  |
| ingress.read.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.read.hosts[0].paths[0].path | string | `"/read"` |  |
| ingress.read.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.read.tls | list | `[]` |  |
| ingress.write.annotations | object | `{}` |  |
| ingress.write.className | string | `""` |  |
| ingress.write.enabled | bool | `false` |  |
| ingress.write.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.write.hosts[0].paths[0].path | string | `"/write"` |  |
| ingress.write.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.write.tls | list | `[]` |  |
| job.annotations | object | `{}` |  |
| keto.autoMigrate | bool | `false` |  |
| keto.config.dsn | string | `"memory"` |  |
| keto.config.namespaces[0].id | int | `0` |  |
| keto.config.namespaces[0].name | string | `"sample"` |  |
| keto.config.serve.read.port | int | `4466` |  |
| keto.config.serve.write.port | int | `4467` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| pdb.enabled | bool | `false` |  |
| pdb.spec.minAvailable | int | `1` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| secret.enabled | bool | `true` |  |
| secret.secretAnnotations."helm.sh/hook" | string | `"pre-install, pre-upgrade"` |  |
| secret.secretAnnotations."helm.sh/hook-delete-policy" | string | `"before-hook-creation"` |  |
| secret.secretAnnotations."helm.sh/hook-weight" | string | `"0"` |  |
| secret.secretAnnotations."helm.sh/resource-policy" | string | `"keep"` |  |
| securityContext.allowPrivilegeEscalation | bool | `false` |  |
| securityContext.capabilities.drop[0] | string | `"ALL"` |  |
| securityContext.privileged | bool | `false` |  |
| securityContext.readOnlyRootFilesystem | bool | `true` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `100` |  |
| service.read.enabled | bool | `true` |  |
| service.read.name | string | `"http-read"` |  |
| service.read.port | int | `80` |  |
| service.read.type | string | `"ClusterIP"` |  |
| service.write.enabled | bool | `true` |  |
| service.write.name | string | `"http-write"` |  |
| service.write.port | int | `80` |  |
| service.write.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| tracing.datadog.enabled | bool | `false` |  |
| watcher.enabled | bool | `false` |  |
| watcher.image | string | `"oryd/k8s-toolbox:0.0.1"` |  |
| watcher.mountFile | string | `""` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)