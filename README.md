# test-service image build process

## Running test-kitchen

```bash
kitchen test
```

## Building images with packer

### Prerequisites

* Vagrant
* Virtualbox
* AWS Credentials

### Building Vagrant Boxes

```bash
packer build packer.vagrant.json
```

### Building AMIs

```bash
packer build packer.aws.json
```
