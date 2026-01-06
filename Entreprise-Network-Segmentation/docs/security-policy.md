# Security Policy

- Admin & IT VLANs have full access to the Server VLAN
- Admin & IT can communicate with each other
- HR & Finance can access Server VLAN only
- HR & Finance are isolated from all other VLANs
- Inter-VLAN routing is implemented using Router-on-a-Stick
- Traffic filtering is enforced using Extended ACLs