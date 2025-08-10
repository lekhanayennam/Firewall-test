# Firewall-test
Configured and tested a custom Windows Firewall rule to block inbound traffic on Telnet port 23. Verified the block using the Telnet client, documented the process with screenshots, and restored the firewall to its original state.
# Task 4 — Windows Firewall Rule Test

## Objective
To configure and test a basic firewall rule to block inbound traffic on a specific port (Telnet — port 23) and verify the block using a Telnet connection attempt.

## Tools Used
- **Windows Defender Firewall with Advanced Security** (built-in tool in Windows)
- **Telnet Client** (installed via Windows Features)

## Steps Followed

### 1. Listed Current Firewall Rules
- Opened **Windows Defender Firewall with Advanced Security**.
- Clicked on **Inbound Rules** to view existing rules.
- Took a screenshot before adding any new rule.

### 2. Added a New Rule to Block Port 23 (Telnet)
- Chose **New Rule** → Selected **Port**.
- Selected **TCP** → Entered port number **23**.
- Selected **Block the connection** → Applied to all profiles (Domain, Private, Public).
- Named the rule **Block Telnet Port 23**.
- Saved the rule and verified it appeared in the list.

### 3. Tested the Rule
- Opened **Command Prompt** and ran:
  ```bash
  telnet localhost 23
