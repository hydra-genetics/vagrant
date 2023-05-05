# Hydra-Genetics Vagrant

Build script for a vagrant machine that can be used by Window/OSX user to run snakemake in combination with singularity.

## Build 

### Dependancies

#### Softwares:
- [VirtualBox](https://www.virtualbox.org/)
- [Vagrant](https://developer.hashicorp.com/vagrant/tutorials/getting-started/getting-started-install)

#### Vagrant plugins:
```bash
vagrant plugin install vagrant-disksize
```

### Build vagrant machine
```bash
cd vagrant_systems/ubuntu/
vagrant up
```

Folder `vagrant_systems/ubuntu/data/` will be mounted into the vagrant machine for easy data sharing.

# Remove machine
```bash
cd vagrant_systems/ubuntu/
vagrant destroy
```

# Enter machine
```bash
cd vagrant_systems/ubuntu/
vagrant ssh

# Liste singularity options
singulariy --help

# Install hydra-genetics
pip install hydra-genetics -y
```


