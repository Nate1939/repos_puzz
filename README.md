Open source BOSH controlled environment based on the design detailed in
[Control Plane Home](https://puzzel.atlassian.net/wiki/spaces/AF/pages/3617161235/Decision+Record+HA+Architecture+for+BOSH+director).

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Access

1. Open VPN connection
2. Connect to the `jumpbox` VM

## Prerequisites

1. `git clone https://puzzel@dev.azure.com/puzzel/automation/_git/bosh-control-plane`
1. `git clone https://puzzel@dev.azure.com/puzzel/automation/_git/bcp-sbx-bosh`
1. Ensure that all scripts are executable by running: `find . -type f -name "*.sh" -exec chmod +x \{\} \;`
1. All commands **MUST** be executed from the repository root!
1. Sufficient access policy to bosh-prod-uks-kv. Must be able to get,list,set,delete,recover,backup and restore secrets.
1. Sufficient access to container within the storage account boshprodukssa. Storage Blob Data Contributor is needed on the "bcp-<env>-bosh-credentials" container.

## Deployment

Please see our [Deployments](docs/deployments.md) page on how to deploy the BOSH Control Plane (BCP) from scratch.

## Deletion

Please see our [Deletion](docs/deployments.md) page on how to delete the BCP.

## Backup & Recovery

Please see our [BBR](docs/bbr.md) page.

## Built With

Visual Studio Code has a [Bosh Editor extension](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-bosh)  available that greatly simplifies working with deployments and cloud configurations.

## Troubleshooting

Please see our [Troubleshooting](docs/troubleshooting.md) page.

## Contributing

Please see our [Contribution](docs/contributing.md) page.


