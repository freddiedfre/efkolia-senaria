# Utility Convinience Script - Open VPN on Google Compute Engine

## Getting Started

### Prerequisites

1. GCP Account (console.google.com)

2. GCE Instance (Google Compute Engine Instance) with either Ubuntu, Debian or CentOS as base image and SSH access enabled.

3. Firewall rule to allow Ingress to UDP port 1194 for GCE instance being used.

### Installation Steps

1. SSH into the GCE instance

2. Ensure all dependecies are up to date

3. Install wget
   - Debian or Ubuntu
   ```
       sudo apt-get install wget
   ```
   - CentOS
   ```
       sudo yum install wget
   ```

4. Fetch and run installation script.
    ```
        sudo wget https://raw.githubusercontent.com/freddiedfre/efkolia-senaria/master/openvpn-gce/install.sh -O openvpn-install.sh && sudo bash openvpn-install.sh
    ```

    NB: Ensure to provide inputs when promted during the scripts execution

5. Configure your local machine to access VPN using the the access credentials and user configurations from step 4

HAPPY VPNing.

