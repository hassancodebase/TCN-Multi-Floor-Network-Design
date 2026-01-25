# VLAN Design Plan

## Overview
To ensure secure and efficient departmental communication, the network uses VLAN-based segmentation. Each department is assigned a unique VLAN, preventing unnecessary broadcast traffic and improving security.

## VLAN Allocation

| VLAN ID | Department           | Purpose |
|-------:|----------------------|---------|
| 10     | Sales                | Sales workstations |
| 20     | Customer Support     | Support team systems |
| 30     | Hardware Department  | Hardware operations |
| 40     | Human Resources      | HR systems |
| 50     | Administration       | Administrative offices |
| 99     | Management & Servers | Core management and servers |

## Trunking Strategy
- All floor switches connect to the core switch (SW-GROUND) using IEEE 802.1Q trunk links.
- The router interface (R1 Gi0/0) is configured as a trunk using sub-interfaces for inter-VLAN routing.

## Benefits
- Logical isolation between departments
- Improved performance by reducing broadcast domains
- Simplified network troubleshooting
- Enhanced security
