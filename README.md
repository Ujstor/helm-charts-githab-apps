# K8s Apps Helm Charts

Helm chart collection that simplifies Kubernetes configuration to be production-ready.

# notes-flask

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.0](https://img.shields.io/badge/AppVersion-1.0.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ujstor/flask-notes"` |  |
| image.tag | string | `"1.0.0"` |  |
| ingress.annotations."cert-manager.io/cluster-issuer" | string | `"letsencrypt"` |  |
| ingress.annotations."nginx.ingress.kubernetes.io/backend-protocol" | string | `"HTTP"` |  |
| ingress.className | string | `"nginx"` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"notes.ujstor.com"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.tls[0].hosts[0] | string | `"notes.ujstor.com"` |  |
| ingress.tls[0].secretName | string | `"notes-flask-tls"` |  |
| nameOverride | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"100m"` |  |
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"50m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| service.port | int | `5010` |  |
| service.targetPort | int | `5010` |  |
| service.type | string | `"ClusterIP"` |  |


![purple-divider](https://user-images.githubusercontent.com/7065401/52071927-c1cd7100-2562-11e9-908a-dde91ba14e59.png)

# portfolio

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.2.3](https://img.shields.io/badge/AppVersion-1.2.3-informational?style=flat-square)

Ujstor's portfolio Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ujstor/portfolio-web-go"` |  |
| image.tag | string | `"1.2.3"` |  |
| ingress.annotations."cert-manager.io/cluster-issuer" | string | `"letsencrypt"` |  |
| ingress.annotations."nginx.ingress.kubernetes.io/backend-protocol" | string | `"HTTP"` |  |
| ingress.className | string | `"nginx"` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"portfolio.ujstor.com"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.tls[0].hosts[0] | string | `"portfolio.ujstor.com"` |  |
| ingress.tls[0].secretName | string | `"portfolio-tls"` |  |
| nameOverride | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"100m"` |  |
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"50m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| service.port | int | `5000` |  |
| service.targetPort | int | `5000` |  |
| service.type | string | `"ClusterIP"` |  |


![purple-divider](https://user-images.githubusercontent.com/7065401/52071927-c1cd7100-2562-11e9-908a-dde91ba14e59.png)

# streamlit-wh

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.1](https://img.shields.io/badge/AppVersion-1.0.1-informational?style=flat-square)

Ujstor's streamlit-wh Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ujstor/working_hours"` |  |
| image.tag | string | `"1.0.1"` |  |
| ingress.annotations."cert-manager.io/cluster-issuer" | string | `"letsencrypt"` |  |
| ingress.annotations."nginx.ingress.kubernetes.io/backend-protocol" | string | `"HTTP"` |  |
| ingress.className | string | `"nginx"` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"working-hours.ujstor.com"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"Prefix"` |  |
| ingress.tls[0].hosts[0] | string | `"working-hours.ujstor.com"` |  |
| ingress.tls[0].secretName | string | `"streamlit-wh-tls"` |  |
| nameOverride | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | string | `"500m"` |  |
| resources.limits.memory | string | `"512Mi"` |  |
| resources.requests.cpu | string | `"250m"` |  |
| resources.requests.memory | string | `"256Mi"` |  |
| service.port | int | `8501` |  |
| service.targetPort | int | `8501` |  |
| service.type | string | `"ClusterIP"` |  |


![purple-divider](https://user-images.githubusercontent.com/7065401/52071927-c1cd7100-2562-11e9-908a-dde91ba14e59.png)

# todo-go-htmx

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.1.0](https://img.shields.io/badge/AppVersion-1.1.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://ujstor.github.io/helm-charts-system | postgres-cluster | 1.0.0 |
| https://ujstor.github.io/helm-charts-system | secret-store | 1.0.0 |

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
| secret-store.secretStore.clusterWide | bool | `false` |  |
| secret-store.secretStore.provider.kubernetes.auth.serviceAccount.create | bool | `true` |  |
| secret-store.secretStore.provider.kubernetes.auth.serviceAccount.name | string | `"todo-secret-store-sa"` |  |
| secret-store.secretStore.provider.type | string | `"kubernetes"` |  |
| service.port | int | `8088` |  |
| service.targetPort | int | `8088` |  |
| service.type | string | `"ClusterIP"` |  |


