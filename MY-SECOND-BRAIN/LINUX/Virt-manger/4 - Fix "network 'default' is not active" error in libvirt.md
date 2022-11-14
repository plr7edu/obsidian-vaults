- When you install QEMU/KVM in Linux, the `default` NAT network is created automatically by `libvirtd` daemon. 

- The properties of the `default` network are defined in the `libvirt`'s default network template (located at `/etc/libvirt/qemu/networks/default.xml`). 

- This `default` network is used to interconnect guest VMs's virtual NICs in NAT mode.

- If, for whatever reason, the `default` network is deactivated, you won't be able to start any guest VMs which are configured to use the network.

When you check the state of existing networks, you will see `inactive` state for the `default` network.


```bash
sudo virsh net-list --all
```

![[275b.jpg]]

Here we show how to solve the `default` network stuck in `inactive` state.

## Solution One : -

Your first attempt can be simply trying to start the network with `virsh`.


```bash
sudo virsh net-start default
```

