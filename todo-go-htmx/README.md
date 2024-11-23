# todo-go-htmx

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.1.0](https://img.shields.io/badge/AppVersion-1.1.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://ujstor.github.io/helm-charts-system | postgres-cluster | 1.0.0 |
| https://ujstor.github.io/helm-charts-system | secstore(secret-store) | 1.0.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ujstor/todo-go-htmx"` |  |
| image.tag | string | `"1.1.1"` |  |
| ingress.annotations."cert-manager.io/cluster-issuer" | string | `"letsencrypt"` |  |
| ingress.annotations."nginx.ingress.kubernetes.io/backend-protocol" | string | `"HTTP"` |  |
| ingress.className | string | `"nginx"` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"todo.ujstor.com"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.tls[0].hosts[0] | string | `"todo.ujstor.com"` |  |
| ingress.tls[0].secretName | string | `"todo-htmx-tls"` |  |
| nameOverride | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| postgres-cluster.instanceCPU | string | `"250m"` |  |
| postgres-cluster.instanceMemory | string | `"500Mi"` |  |
| postgres-cluster.instanceReplicas | int | `1` |  |
| postgres-cluster.instances[0].dataVolumeClaimSpec.accessModes[0] | string | `"ReadWriteOnce"` |  |
| postgres-cluster.instances[0].dataVolumeClaimSpec.resources.requests.storage | string | `"100Mi"` |  |
| postgres-cluster.instances[0].name | string | `"todo-htmx-go"` |  |
| postgres-cluster.instances[0].replicas | int | `1` |  |
| postgres-cluster.patroni.dynamicConfiguration.postgresql.pg_hba[0] | string | `"local all postgres trust"` |  |
| postgres-cluster.patroni.dynamicConfiguration.postgresql.pg_hba[1] | string | `"local all all trust"` |  |
| postgres-cluster.patroni.dynamicConfiguration.postgresql.pg_hba[2] | string | `"host all all all md5"` |  |
| postgres-cluster.pgBackRestConfig.repos[0].name | string | `"repo1"` |  |
| postgres-cluster.pgBackRestConfig.repos[0].volume.volumeClaimSpec.accessModes[0] | string | `"ReadWriteOnce"` |  |
| postgres-cluster.pgBackRestConfig.repos[0].volume.volumeClaimSpec.resources.requests.storage | string | `"100Mi"` |  |
| postgres-cluster.pgBackRestConfig.resources.limits.cpu | string | `"50m"` |  |
| postgres-cluster.pgBackRestConfig.resources.limits.memory | string | `"64Mi"` |  |
| postgres-cluster.port | int | `5432` |  |
| postgres-cluster.postgresVersion | int | `16` |  |
| postgres-cluster.users[0].databases[0] | string | `"todo-go-htmx"` |  |
| postgres-cluster.users[0].name | string | `"todo-go-htmx"` |  |
| postgres-cluster.users[0].options | string | `"SUPERUSER"` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"100m"` |  |
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"50m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| secstore.secretStore.clusterWide | bool | `false` |  |
| secstore.secretStore.provider.kubernetes.auth.serviceAccount.create | bool | `true` |  |
| secstore.secretStore.provider.kubernetes.auth.serviceAccount.name | string | `"todo-secret-store-sa"` |  |
| secstore.secretStore.provider.type | string | `"kubernetes"` |  |
| service.port | int | `8088` |  |
| service.targetPort | int | `8088` |  |
| service.type | string | `"ClusterIP"` |  |

