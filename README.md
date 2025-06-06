# VPN Task 8: Understanding and Using VPNs for Privacy and Secure Communication

## Objective

The aim of this task was to gain practical experience with Virtual Private Networks (VPNs), focusing on their role in enhancing online privacy and securing communication. The task involved setting up and using a VPN client on Kali Linux, verifying IP masking, and analyzing encrypted traffic behavior.

## Tools Used

- **VPN Client:** ProtonVPN (Free Tier)
- **Operating System:** Kali Linux
- **Web Browser:** Brave
- **Command Line Tools:** `sudo apt`, `wget`, `curl`, `dpkg`, `ip`, `protonvpn-cli`

## VPN Setup & Configuration

1. **Service Selection & Account Creation**
   - Chose [ProtonVPN](https://protonvpn.com) (Free Tier) for its privacy-first approach.
   - Created a free account on their official website.

2. **Client Installation on Kali Linux**
   - Removed old ProtonVPN configs.
   - Downloaded and installed the release package via `wget` and `dpkg`.
   - Verified and configured GPG keys.
   - Reinstalled and updated using `apt`.

3. **Connecting to VPN**
   - Initialized setup:  
     ```bash
     sudo protonvpn-cli init
     ```
   - Connected to fastest server:  
     ```bash
     sudo protonvpn-cli c -f
     ```

## Verifying Connection

- Visited [whatismyipaddress.com](https://whatismyipaddress.com) via Brave browser.
- Confirmed IP change to `49.43.3.21` (Mumbai, India).
- Verified encrypted tunnel by browsing multiple websites without disruption.


