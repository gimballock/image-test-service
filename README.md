# test-service image build process

## Running test-kitchen

```bash
kitchen test
```
### Testing cookbooks

In the root of the project:
* to execute rubocop: `rubocop .`
* to execute foodcritic: `foodcritic .`
* to execute chefspec: `rspec spec`
* to execute test kitchen: `kitchen test`

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
