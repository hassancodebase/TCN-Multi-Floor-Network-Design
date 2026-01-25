# IP Addressing Plan (VLSM)

## Base Network
- Network: 199.99.99.0/24
- Subnetting Method: Variable Length Subnet Masking (VLSM)

## Subnet Allocation

| Department           | Hosts | Subnet              | Gateway |
|----------------------|------:|---------------------|---------|
| Sales                | 27    | 199.99.99.0/27      | .1 |
| HR                   | 25    | 199.99.99.32/27     | .33 |
| Customer Support     | 16    | 199.99.99.96/27     | .97 |
| Administration       | 10    | 199.99.99.128/28    | .129 |
| Hardware              | 20   | 199.99.99.160/27    | .161 |
| Management/Servers   | N/A   | 199.99.99.144/28    | .145 |

## Address Assignment
- All workstations receive IP addresses dynamically via DHCP.
- Gateway IPs are excluded from DHCP pools.
- DNS Server: 199.99.99.146 (Web Server)

## Advantages
- Efficient use of IP space
- Minimal address wastage
- Easy scalability for future departments
