# vagrant-fusion-osx


http://www.skoblenick.com/vagrant/vmware-fusion/creating-an-osx-base-box/
Updating the OS
- sudo softwareupdate --install --all


Disable the Firewall in OS X
- Navigate to System Preferences > Security & Privacy.
- Select the Firewall tab view.
- Ensure the Firewall is Off


Enabling Remote Login
- Navigate to System Preferences > Sharing.
- Check Remote Login to turn it On
- Optional. Change the access permissions as necessary. All Users is selected by default. If you change this option to Only these users:, add the vagrant user you created.


Download Vagrant’s insecure key
$ mkdir -p /Users/vagrant/.ssh
$ chmod 0700 /Users/vagrant/.ssh
$ curl -o /Users/vagrant/.ssh/authorized_keys --url https://raw.github.com/mitchellh/vagrant/master/keys/vagrant.pub
$ chmod 0600 /Users/vagrant/.ssh/authorized_keys
$ chown -R vagrant /Users/vagrant/.ssh
