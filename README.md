# NETTOOLS- Advanced Cybersecurity Toolkit 🔒

![Nettools Banner]

A multi-functional Python-based networking and security assessment tool with both command-line and interactive modes, designed for ethical hacking, penetration testing, and network diagnostics.

## FEATURES ✨

- **Dual Interface Mode**
  - Interactive menu system
  - Traditional command-line arguments
- **Network Scanning**
  - Multi-threaded port scanning (100+ threads)
  - Service banner grabbing
  - Vulnerability detection (CVE checking)
  - Local network device discovery (ARP scanning)
- **IP Analysis**
  - Public/private IP identification
  - IP geolocation
  - Reverse DNS lookup
  - IP validation
- **Domain Intelligence**
  - WHOIS lookups
  - DNS A record resolution
- **User Experience**
  - Color-coded terminal output
  - Progress indicators
  - Detailed reporting

## INSTALLATION ⚙️

### Requirements
- Python 3.6+
- Root/admin privileges (for network scanning)

### Setup
```bash
# Clone repository
git clone https://github.com/yourusername/nettools.git
cd nettools
# Install dependencies
pip install -r requirements.txt
## Complete Usage Examples 💻

```

## USAGE
### NETWORK INFORMATION
```bash
#### Get private IP addresses
python Nettools_Version2.py private-ip

#### Get public IP address 
python Nettools_Version2.py public-ip

#### Validate an IP address
python Nettools_Version2.py validate-ip 8.8.8.8

##### IP geolocation lookup
python Nettools_Version2.py geoip 1.1.1.1

##### Reverse DNS lookup
python Nettools_Version2.py reverse-dns 8.8.8.8

### SCANNING TOOLS
#### Basic port scan (default 1-1024 ports)
python Nettools_Version2.py port-scan 192.168.1.1

#### Advanced port scan with custom range and threads
python Nettools_Version2.py port-scan 192.168.1.1 --ports 20-500 --threads 200

#### Grab service banner from specific port  
python Nettools_Version2.py banner-grab 192.168.1.1 80

#### Scan local network for devices
python Nettools_Version2.py netscan 192.168.1.0/24

### DOMAIN TOOLS  
#### WHOIS lookup
python Nettools_Version2.py whois google.com

#### DNS A record lookup
python Nettools_Version2.py dns example.com
```

## INTERACTIVE MODE

```bash
### Launch interactive menu system
python Nettools_Version2.py
```

## COMMAND MODE (from within interactive)
```bash
nettools> port-scan 10.0.0.1 --ports 1-100
nettools> whois microsoft.com
nettools> back  # Return to main menu
```
