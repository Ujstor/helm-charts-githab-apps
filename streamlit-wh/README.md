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
| ingress.tls.secretName | string | `nil` |  |
| ingressClassName | string | `nil` |  |

