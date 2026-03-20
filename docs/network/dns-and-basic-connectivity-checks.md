# DNS and Basic Connectivity Checks

## Objective
Provide simple connectivity tests before escalating network issues.

## Basic Tests
- Check local IP address
- Confirm default gateway is assigned
- Ping gateway if permitted
- Test access to a public website
- Test access to internal hostname
- Compare results using hostname versus IP address

## Interpretation
- Public sites fail: likely internet or broader network issue
- Public works, internal fails: possible VPN, DNS, or internal routing issue
- IP works but hostname fails: likely DNS issue

## Escalate When
- Repeated DNS failures affect multiple users
- Internal name resolution fails after standard checks
- Routing or firewall issue is suspected