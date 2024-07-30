# README

## Vagrant Setup for WordPress Environment

This Vagrant setup creates a virtual machine (VM) using the Ubuntu Focal64 box. The VM is configured to set up a WordPress environment with Apache, PHP, and MySQL using a bash script.

### Prerequisites

- [Vagrant](https://www.vagrantup.com/downloads)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

### Features

- **OS**: Ubuntu Focal64
- **Private Network IP**: 192.168.56.30
- **Memory**: 1600 MB
- **Software Installed**:
  - Apache
  - MySQL
  - PHP and various PHP extensions
  - WordPress

### Provisioning

The VM is provisioned with a shell script that:
1. Updates the package list and installs necessary packages.
2. Sets up Apache with the necessary modules and configures a WordPress site.
3. Creates a MySQL database and user for WordPress.
4. Configures WordPress settings.

### How to Use

1. Clone the repository containing the Vagrantfile.
2. Navigate to the directory containing the Vagrantfile.
3. Run `vagrant up` to start and provision the VM.
4. Access the WordPress setup by navigating to the private network IP in your browser (http://192.168.56.30).

### Additional Information

- The VM includes a provision script for setting up a WordPress environment. You can customize the provision script as needed.
- Port forwarding and other network configurations can be adjusted in the Vagrantfile.

For more details, refer to the [Vagrant documentation](https://www.vagrantup.com/docs).

