# Model Notes

## Introduction

The inspiration of this repo is to take some of the best parts of the NetBox & the various community Plugins models to create a more comprehensive model that can be used for a variety of use cases.

## Reference Models

- [InfraHub Schema Library](https://github.com/opsmill/schema-library)
- [NetBox](https://github.com/netbox-community/netbox)
- [NetBox Plugin - BGP](https://github.com/netbox-community/netbox-bgp)
- [NetBox Plugin - Circuit Maintenance](https://github.com/jasonyates/netbox-circuitmaintenance)
- [NetBox Plugin - Cisco Support](https://github.com/goebelmeier/netbox-cisco-support)
- [NetBox Plugin - Contract](https://github.com/mlebreuil/netbox-contract)
- [NetBox Plugin - Contract](https://github.com/mlebreuil/netbox-contract)
- [NetBox Plugin - EVPN VC](https://github.com/zarya/netbox-evpn-vc)
- [NetBox Plugin - Gateways](https://github.com/ITJamie/netbox_gateways)
- [NetBox Plugin - Inventory](https://github.com/ArnesSI/netbox-inventory)
- [NetBox Plugin - Lifecycle](https://github.com/DanSheps/netbox-lifecycle)
- [NetBox Plugin - OS Manager](https://github.com/jonasnieberle/netbox-os-manager)
- [NetBox Plugin - PhoneBox](https://github.com/iDebugAll/phonebox_plugin)
- [NetBox Plugin - DNS](https://github.com/peteeckel/netbox-plugin-dns)
- [NetBox Plugin - MCLAG](https://github.com/pv2b/netbox-plugin-mclag)
- [NetBox Plugin - Routing](https://github.com/DanSheps/netbox-routing)
- [NetBox Plugin - Software Lifecycle Management](https://github.com/ICTU/netbox_slm)
- [NetBox Plugin - Software Manager](https://github.com/alsigna/netbox-software-manager)
- [NetBox Plugin - Static Routes](https://github.com/jbparrish17/netbox-static-routes)

## Phase 1

### Organization

Not looking to mess around with the organization model too much. It's pretty solid as is.

- Sites
- Regions
- Site Roles (Rename NetBox Site Groups)
- Locations
- Contact Groups
- Contacts
- Contact Roles
- Contact Assignments?

### Devices

- Device Models (Rename NetBox Device Types)
- Device Roles
- Platforms
- Device Clusters
- Device Virtual Chassis (includes stacks)
- Device MLAG/VPC Group
- Manufacturers

### IPAM

- IPAM Roles
- IPs
- IP Ranges
- Prefixes
- VRFs
- ASNs (Move to Routing Phase 2)
- ASN Ranges (Move to Routing Phase 2)
- Aggregates
- RIRs
- VLANs
- VLAN Groups
- Communities (Move to Routing Phase 2)
- Community Lists (Move to Routing Phase 2)

### Connectivity

Look to rename circuits to something more generic like connectivity.

- Connectivity Providers
- Connectivity Services (Renamed from Circuits)
- Provider Networks
- Connectivity Types
- Connectivity Terminations
- Provider Accounts (made into generic accounts?)

## Phase 2

### Infra Lifecycle

- Hardware LifeCycle (EOL/EOS)
- Softare LifeCycle (EOL/EOS)
- Software Images
- Validated Software

### Connectivity (Phase 2)

- Connectivity Maintenances
- Connectivity Notifications

### Routing

- BGP
  - Sessions
  - Peer Groups
  - Communities
  - Community Lists
  - ASNs
  - ASN Ranges
  - Prefix Lists
  - Prefix List Entries
  - Route Maps
  - Route Map Entries
  - Routing Policies

### DNS

- Domains
- Domain Registrars
- Name Servers
- Records
  - AAA Records
  - C Names
  - MX Records

### Devices (Phase 2)

- Modules
- Interfaces
- Module Types
- Interface Types
- Interface Roles
- Device Bays

## Phase 3

### Designs

- Interface Profiles
- Toplogies

### Contracts

- Support
- License

### Inventory

- Inventory Items
- Consumables (Need a way to decrement a quantity easily)

### Cloud

- Direct Connects
- Cloud Providers
- Cloud Accounts
- Cloud Regions
