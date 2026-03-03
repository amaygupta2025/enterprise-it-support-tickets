# VPN Configuration for MSP Remote Access

## Type
Service Request

## Objective
Enable secure VPN access on the MSP-Helpdesk workstation for after-hours support.

## Environment
- Windows 10
- Corporate VPN Client
- Domain credentials + MFA

## Actions Performed
1. Installed corporate-approved VPN client.
2. Configured VPN profile with company gateway.
3. Enabled domain authentication with MFA.
4. Established VPN connection.
5. Verified assigned VPN IP using `ipconfig`.
6. Confirmed internal DNS resolution.
7. Tested access to file server and intranet portal.

## Validation
- VPN connected successfully.
- Internal resources accessible.
- No authentication or DNS issues observed.

## Outcome
VPN configured and validated. MSP can securely access internal systems for after-hours support.
