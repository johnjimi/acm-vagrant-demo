## Vagrant How-To

The steps of the Vagrant file are in the branches

- Vagrant: [www.vagrantup.com](https://github.com/davidnuon/acm-vagrant-demo)
- VirtualBox: [www.virtualbox.org](https://www.virtualbox.org/wiki/Downloads)

Example of a useful box:
- Scotchbox: [https://box.scotch.io/](https://box.scotch.io/)

After installing both Vagrant and VirtualBox:
- Choose a directory.
- For Macs: Run terminal and type command 'vagrant box add [box name]' to add box
  for this example: type command 'vagrant box add scotch/box'
- After the download is complete type command 'vagrant init [box name]' e.g. 'vagrant init scotch/box'
- Type command 'vagrant up' and you are set.
