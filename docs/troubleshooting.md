# Troubleshooting & Issues Resolved

## Common Issues Encountered

### VLAN Communication Failure
**Cause:** VLANs not created on SW-GROUND  
**Fix:** Manually created VLANs and verified trunk propagation

### Trunk Ports Not Carrying VLANs
**Cause:** Incorrect allowed VLAN list  
**Fix:** Updated trunk configuration to allow required VLANs

### No Internet Connectivity
**Cause:** Cloud-PT interface misconfiguration  
**Fix:** Assigned correct IP address to Cloud Ethernet interface

### IP Address Conflicts
**Cause:** Incorrect VLSM calculations  
**Fix:** Recalculated subnet sizes and updated DHCP pools

### Email Communication Failure
**Cause:** Incorrect domain and user configuration  
**Fix:** Corrected DNS records and email server user accounts

## Verification Methods
- Ping tests across VLANs
- DHCP binding verification
- Server reachability tests
- Email send/receive validation
