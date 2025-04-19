# Confidential Deepfake Detection Demo

## Overview
This repository demonstrates how to deploy a deepfake detection service with end-to-end confidentiality using Tinfoil's confidential computing platform. It showcases how existing AI applications can be made confidential with minimal code changes.

## What is Tinfoil?
Tinfoil is a platform that enables confidential computing for AI applications. It allows you to deploy your existing AI models inside secure confidential VMs where data remains encrypted even during processing, creating an end-to-end confidential environment.

## Repository Structure
- `confidential-df-demo/`: Main repository that orchestrates the confidential deployment
  - Contains configuration for deploying the deepfake detection server inside a confidential VM
  - Includes Tinfoil-specific setup for secure enclave configuration

## Prerequisites
- Docker
- Access to Tinfoil's confidential computing platform

## How It Works
This repository takes the standard deepfake detection server code from the `df-demo` repository and deploys it inside a Tinfoil confidential VM. The deployment process:

1. Packages the existing Docker image in a confidential environment
2. Sets up secure communication channels
3. Provides an enclave URL for client applications to connect securely 

## Security Benefits
- **Data Confidentiality**: All video data remains encrypted, even during processing
- **Secure Execution**: The AI model runs in a trusted execution environment
- **Zero Trust**: Not even cloud providers can access the sensitive data

## Related Repositories
- [df-demo](https://github.com/tinfoilsh/df-demo): The core deepfake detection server
- [df-demo-client](https://github.com/tinfoilsh/df-demo-client): Client application that connects to the confidential deepfake detection service

## Contact
For more information about Tinfoil's confidential computing platform, visit [tinfoil.sh](https://tinfoil.sh)
