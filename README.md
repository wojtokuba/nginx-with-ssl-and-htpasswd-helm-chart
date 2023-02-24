<!--- app-name: NGINX Open Source -->

# NGINX Open Source modified by Jakub Wojtowicz

## TL;DR

This is a thiner version of bitnami Nginx Helm chart without metrics and other monitoring features.
We've added the following extra features for example for lab usages:

- Easy htaccess management directly from your `values.yaml`
- SSL certificate with selfsigned option and/or certificates as variables
- PersistentVolumeClaim for your data mounted in `/app` path

Simply install it with: 

```console
helm repo add bitnami https://charts.bitnami.com/bitnami
helm dependency build
helm install nginx-test ./
```

## Introduction

Bitnami charts for Helm are carefully engineered, actively maintained and are the quickest and easiest way to deploy containers on a Kubernetes cluster that are ready to handle production workloads.

This chart bootstraps a [NGINX Open Source](https://github.com/bitnami/containers/tree/main/bitnami/nginx) deployment on a [Kubernetes](https://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

Bitnami charts can be used with [Kubeapps](https://kubeapps.dev/) for deployment and management of Helm Charts in clusters.

## Prerequisites

- Kubernetes 1.19+
- Helm 3.2.0+

## Bitnami Kubernetes Documentation

Bitnami Kubernetes documentation is available at [https://docs.bitnami.com/](https://docs.bitnami.com/). You can find there the following resources:

- [Documentation for NGINX Helm chart](https://docs.bitnami.com/kubernetes/infrastructure/nginx/)
- [Get Started with Kubernetes guides](https://docs.bitnami.com/kubernetes/)
- [Bitnami Helm charts documentation](https://docs.bitnami.com/kubernetes/apps/)
- [Kubernetes FAQs](https://docs.bitnami.com/kubernetes/faq/)
- [Kubernetes Developer guides](https://docs.bitnami.com/tutorials/)

## License

Copyright &copy; 2023 Bitnami

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.