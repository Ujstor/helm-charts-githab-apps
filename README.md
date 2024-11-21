# K8s Apps Helm Charts

Helm chart collection that simplifies Kubernetes configuration to be production-ready.


# portfolio

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.2.3](https://img.shields.io/badge/AppVersion-1.2.3-informational?style=flat-square)

Ujstor's portfolio Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| deployment.image | string | `"ujstor/portfolio-web-go"` |  |
| deployment.replicas | string | `nil` |  |
| deployment.tag | string | `"1.2.3"` |  |
| domain | string | `"portfolio.ujstor.com"` |  |
| ingress.issuer | string | `nil` |  |
| ingress.tls.secretName | string | `nil` |  |
| ingressClassName | string | `nil` |  |


![purple-divider](https://user-images.githubusercontent.com/7065401/52071927-c1cd7100-2562-11e9-908a-dde91ba14e59.png)



![purple-divider](https://user-images.githubusercontent.com/7065401/52071927-c1cd7100-2562-11e9-908a-dde91ba14e59.png)


# streamlut-wh

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.1](https://img.shields.io/badge/AppVersion-1.0.1-informational?style=flat-square)

Ujstor's streamlut-wh Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| deployment.image | string | `"ujstor/working_hours"` |  |
| deployment.replicas | string | `nil` |  |
| deployment.tag | string | `"1.0.1"` |  |
| domain | string | `"working-hours.ujstor.com"` |  |
| ingress.issuer | string | `nil` |  |
