# iot-cluster-iac

The purpose of this solution is to deploy a Kubernetes cluster to utilize for Device Simulations.

[![Build Status](https://dascholl.visualstudio.com/IoT/_apis/build/status/danielscholl.iot-cluster-iac?branchName=master)](https://dascholl.visualstudio.com/IoT/_build/latest?definitionId=25&branchName=master)

__PreRequisites__

Requires the use of [direnv](https://direnv.net/).  
Requires the use of [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest).  
Requires the use of [Docker](https://www.docker.com/get-started).  


### Related Repositories

- [iot-resources](https://github.com/danielscholl/iot-resources)  - Deploying IoT Resources and x509 Management
- [iot-device-edge](https://github.com/danielscholl/iot-device-edge) - Simple Edge Testing
- [iot-device-js](https://github.com/danielscholl/iot-device-js) - Simple Device Testing (NodeJS)
- [iot-device-js](https://github.com/danielscholl/iot-device-net) - Simple Device Testing (C#)
- [iot-control-js](https://github.com/danielscholl/iot-control-js) - Simple Control Testing


## Getting Started

1. Run Install Script for ARM Process

> Requires manually copying in the SSH Key that is created at this time.

```bash
# Initialize the Modules
contact="<your_initials>"
install.sh $contact
```


# Build and Test 

>NOTE:  THIS CAN ONLY BE DONE FROM A LINUX SHELL!!

1. Manually run the test suite

```bash
npm install
npm test
```

2. Manually provision the infrastructure.

```bash
# Provision the infrastructure
npm run provision
```
