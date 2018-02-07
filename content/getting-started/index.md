---
date: 2017-01-09T00:11:02+01:00
title: Getting started
prev: /
weight: 20
---

## Dependencies

DevSecOps Studio uses `vagrant`, `virtualbox` and `ansible` to setup the lab environment. You can visit the vendor's website to download the above software for on Windows/Linux/macOS.

DevSecOps Studio simulates the environment presented below.

![Appsec Pipeline](/images/appsec-pipeline.png)


### Software

* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
* [Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html#installation)

### Hardware
* Atleast 4GB of RAM for the virtual machines.
* 60GB of HDD Space.
* Intel i3 Processor or above.

## MacOS Installation 

Prerequisites can also be installed via homebrew on MAC OS X

[Homebrew](http://brew.sh/): Optional

```bash
 /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

```

[Vagrant](https://www.vagrantup.com/downloads.html)

```bash
brew cask install vagrant
```

[Virtualbox](https://www.virtualbox.org/wiki/Downloads)

```bash
brew cask install virtualbox
```

[Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html#installation)

``` bash
brew install ansible
```

## Linux Installation
Install dependencies using apt-get

[Virtualbox](https://www.virtualbox.org/wiki/Downloads)

``` bash
sudo sh -c 'echo "deb http://download.virtualbox.org/virtualbox/debian xenial contrib" >> /etc/apt/sources.list.d/virtualbox.list'

wget -q https://www.virtualbox.org/download/oracle_vbox_2016.asc -O- | sudo apt-key add -

sudo apt update

sudo apt install virtualbox
```
[Vagrant](https://www.vagrantup.com/downloads.html)

``` bash
sudo apt-get install vagrant python2 python2-pip
```
[Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html#installation)

``` bash
pip install ansible
```

## Windows Installation

Alternatively, Installation can be done using [chocolatey](https://chocolatey.org/install) by opening up command prompt  and using the following command.

```bash
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

Install dependencies using choco

```bash
choco install vagrant virtualbox git
```

Install ansible via pip

```bash
choco install python --version 2.7.6
pip install ansible
```

## Installation 

1. Clone this repo or download the zip

	```bash
	$ git clone https://github.com/teacheraio/DevSecOps-Studio.git
	```

1. CD into the directory and check what boxes are available.

	```bash
	$ cd DevSecOps-Studio && vagrant status
	```
2. Download requirement ansible dependencies.
    ```bash
    $ ansible-galaxy install -r requirements.yml
    ```

## Configuration

If you wish to make any changes to default setup, please edit `machines.yml` . Meanwhile, go grab some coffee to enjoy.

 ``` bash
 vagrant up
 ```
You can see how it all fits in DevSecOps pipeline by reading out [wiki](https://github.com/teacheraio/DevSecOps-Studio/wiki)
