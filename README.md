# K8s Apps Helm Charts

Helm chart collection that simplifies Kubernetes configuration to be production-ready.


# portfolio

![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.23.0](https://img.shields.io/badge/AppVersion-1.23.0-informational?style=flat-square)

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
