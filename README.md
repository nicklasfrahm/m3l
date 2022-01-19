# M3L ⚙️

M3L is a suite of microservices for software-defined networking (SDN) and bare-metal provisioning, which store their data as Custom Resources in Kubernetes.

## Components 📦

- `m3l-dhcp`  
  A DHCP server that runs within Kubernetes and provides DHCP via the `Fabric` Custom Resource. A `Fabric` may define policies for which DHCP clients are allowed to obtain IP addresses.

- `m3l-snmp`  
  A software-defined networking (SDN) controller, which watches the `Lease` Custom Resource and reconciles VLANs according to the `Fabric` Custom Resource. It uses SNMP to configure the VLANs.

## License 📄

This project is and will always be licensed under the terms of the [MIT license](./LICENSE.md).
