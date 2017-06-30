<h3/>
# Install & setup ovs on stationary/ethernet alpine based libvirt/qemu host
<h2/

## Install OVS packages & dependencies for build
      $ apk add openvswitch openvswitch-doc openvswitch-dev openvswitch-bash-completion

## Start OVS VSwitchDaemon & Add to Default Run Level
      $ rc-update add ovs-vswitchd default
      $ rc-service ovs-vswitchd start

