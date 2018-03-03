# puppetanirbeginer


# to install puppet go to yum.puppetlabs.com to take the repositories select https://yum.puppetlabs.com/puppetlabs-release-pc1-el-7.noarch.rpm the enterprise architecture linux 7 the install with prm -ivh and the link do on master and node and on the master run the command yum -y install puppetserver and on the node run yum -y install puppet-agent

# once installed if we run puppet it will not show anything as puppet binary is not in a path. the reason the binaries are installed in ls -l /opt/puppetlabs/bin and few other in ls -l /opt/puppetlabs/puppet/bin . so we have to add them to our path variable by going to vim /etc/profile.d/puppet-agent.sh so add export PATH=$PATH:/opt/puppetlabs/puppet/bin do this on all the systems then logout and login then we can see the puppet binaries are available

# once the installation is done we can check with cmd rpm -q puppet-agent and puppet --version
