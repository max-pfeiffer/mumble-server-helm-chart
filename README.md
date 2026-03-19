[![Lint Helm Chart](https://github.com/max-pfeiffer/mumble-server-helm-chart/actions/workflows/helm-lint.yaml/badge.svg)](https://github.com/max-pfeiffer/mumble-server-helm-chart/actions/workflows/helm-lint.yaml)
[![Release Helm Charts](https://github.com/max-pfeiffer/mumble-server-helm-chart/actions/workflows/helm-release.yaml/badge.svg)](https://github.com/max-pfeiffer/mumble-server-helm-chart/actions/workflows/helm-release.yaml)

# Mumble Server Helm Chart
Helm chart for [Mumble server](https://www.mumble.info/).

This Helm chart runs [Mumble server](https://www.mumble.info/) as Statefulset with SQLite database.
As this application does not seem to scale horizontally.  

## Installation
The installation is done as follows:
```shell
$ helm repo add mumble-server https://max-pfeiffer.github.io/mumble-server-helm-chart
$ helm install mumble-server mumble-server/mumble-server --values your_values.yaml --namespace yournamespace 
```

## Additional Information Sources
* [Mumble Docker Image](https://github.com/mumble-voip/mumble-docker)
* [mumble-server.ini](https://github.com/mumble-voip/mumble/blob/master/auxiliary_files/mumble-server.ini)