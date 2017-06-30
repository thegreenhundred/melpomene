<h1/>
Install & setup ovs on stationary/ethernet alpine based libvirt/qemu host

## Install OVS packages & dependencies for build
      $ apk add openvswitch openvswitch-doc openvswitch-dev openvswitch-bash-completion

## Start OVS VSwitchDaemon & Add to Default Run Level
      $ rc-update add ovs-vswitchd default
      $ rc-service ovs-vswitchd start

## Initialize the ovs database
sudo ovs-vsctl init
ovs-vsctl add-br $BR1NAME
