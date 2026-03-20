# VPN Troubleshooting Flow

## Common Symptoms
- VPN client will not connect
- MFA prompt does not arrive
- Connected but cannot access internal resources
- Frequent disconnects
- VPN works on one network but not another

## Troubleshooting Steps
1. Confirm internet access without VPN
2. Ask for exact error message or screenshot
3. Confirm username and password work for standard sign-in
4. Verify MFA method is working
5. Confirm VPN client version is current
6. Restart the device and retry
7. Test on alternate network if available
8. Check whether DNS/internal resources resolve after connection
9. Verify account is permitted for VPN access
10. Escalate if client configuration or gateway issue is suspected

## Escalate When
- VPN gateway or certificate issue is suspected
- Multiple users report same problem
- User authenticates successfully but cannot reach internal services
- Client logs indicate infrastructure-side failure