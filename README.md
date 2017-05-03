# vagrant
<br />
<b>What is Vagrant?</b>
<p>Vagrant is virtualization tool to create virtual environment for development on your system. It is open source software widely used for development purpose like install any new release of operating system, any new application or installing updates for testing any new feature , as things need to tested before taking it to production enviroment.</p>

<h3>Steps to install and run vagrant</h3>
<p><b>Note:</b> Before installing make sure to install VirtualBox on your machine.</p>
<dl>
  <dt>Installing Vagrant on Ubuntu 14.04</dt>
  <dd>-> sudo apt-get install vagrant</dd>
  <dt>Installing Vagrant on CentOs</dt>
  <dd>$ wget https://dl.bintray.com/mitchellh/vagrant/vagrant_1.4.2_x86_64.rpm -O vagrant_1.4.2_x86_64.rpm<br/>
      $ sudo rpm -i vagrant_1.4.2_x86_64.rpm<br />$ vagrant -v <br /> $ vagrant -h </dd>
</dl>

<h3>Creating Vagrant Box </h3>
<ul>
<li>Create a directory in your home or any directory. eg- <b><br/>$ mkdir centos-box</b></li>
<li>Change to new directory <b><br />$ cd centos-box</b></li>
<li>Copy vagrant box url from <a href="http://www.vagrantbox.es/">VagrantBox</a>  <b><br />$ vagrant box add centos http://developer.nrel.gov/downloads/vagrant-boxes/CentOS-6.4-i386-v20131103.box</b></li>
<li>Initialize vagrant Box <b><br/>$ vagrant init centos</b></li>
<li>Start vagrant Box <b><br/>$ vagrant up</b></li>
</ul>
Use <a href="http://www.vagrantbox.es/">VagrantBox</a> to copy required box <b>url</b> e.g. environment which you want to create using vagrant like Ubuntu, CentOs
<br />
 $ vagrant box add {title} {url}<br />
 $ vagrant init {title}<br />
 $ vagrant up<br />
 
 <h4>Basic Vagrant Command</h4>
 <ul>
 <li>Destroys the Droplet instance. <b><br />$ vagrant destroy </b> </li>
 <li>Logs into the Droplet instance using the configured user account. <b><br />$ vagrant ssh </b></li>
 <li>Powers off the Droplet instance. <b><br />$ vagrant halt </b></li>
 <li>Runs the configured provisioners and rsyncs any specified config.vm.synced_folder.<b><br />$ vagrant provision</b> </li>
 <li>Reboots the Droplet instance. <b><br />$ vagrant reload </b></li>
 <li>Destroys the Droplet instance and recreates it with the same IP address which was previously assigned. <b><br />$ vagrant rebuild </b></li>
 <li> Outputs the status (active, off, not created) for the Droplet instance.<b><br />$ vagrant status </b></li>
 </ul>
