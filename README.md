# Helm Chart for smtp4dev

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![version](https://img.shields.io/github/tag/IMIO/helm-smtp4dev.svg?label=release) ![test](https://github.com/IMIO/helm-smtp4dev/actions/workflows/test.yaml/badge.svg) ![release](https://github.com/IMIO/helm-smtp4dev/actions/workflows/release.yaml/badge.svg)

## Introduction

This [Helm](https://helm.sh/) chart installs [smtp4dev](https://github.com/rnwood/smtp4dev) in a [Kubernetes](https://kubernetes.io) cluster.

## Prerequisites

- Kubernetes cluster 1.19+
- Helm 3.0.0+
- PV provisioner support in the underlying infrastructure (Optional)

## Installation

### Add Helm repository

```bash
helm repo add imio https://imio.github.io/helm-charts
helm repo update
```

### Configure the chart

The following items can be set via `--set` flag during installation or configured by editing the `values.yaml` directly (need to download the chart first).

Feel free to modify the options in the [values.yaml file](values.yaml) before installation.

### Install the chart

```bash
helm install [RELEASE_NAME] imio/smtp4dev
```

or by cloning this repository:

```bash
git clone https://github.com/imio/helm-smtp4dev.git
cd helm-smtp4dev
helm install smtp4dev . -f values.yaml --namespace smtp4dev --create-namespace
```

## Configuration

The following table lists the configurable parameters of the smtp4dev chart and the default values.

See the [values.yaml](values.yaml) file for more information.

## Contributing

Feel free to contribute by making a [pull request](https://github.com/imio/helm-smtp4dev/pull/new/master).

Please read the official [Helm Contribution Guide](https://github.com/helm/charts/blob/master/CONTRIBUTING.md) from Helm for more information on how you can contribute to this Chart.

## License

[Apache License 2.0](/LICENSE)
