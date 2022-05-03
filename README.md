# kubernetes_vagrant


1. Install VirtualBox
sudo yum –y install epel-release
sudo yum –y install gcc dkms make qt libgomp patch
sudo yum –y install kernel-headers kernel-devel binutils glibc-headers glibc-devel font-forge
sudo wget http://download.virtualbox.org/virtualbox/rpm/rhel/virtualbox.repo -o /etc/yum.repo.d/
sudo yum –y install VirtualBox-5.2

2. Install Vagrant on CentOS
sudo yum update
sudo wget https://releases.hashicorp.com/vagrant/2.2.2/vagrant_2.2.2_x86_64.rpm
sudo yum –y localinstall vagrant_2.2.2_x86_64.rpm
vagrant ––version

3. Vagrant on CentOS
sudo mkdir -p /vagrant/{master, worker1,worker2}
cd /vagran/{master, worker1,worker2}
touch Vagrantfile
vagrant up

Here there are 3 vagrant file which can be use to create 1 master and 2 worker node. vagrant files naming convention are set according to that.

To create thsoe VMs need to rename these file names to Vagrantfile only in vagrant's specific location to up the servers.

