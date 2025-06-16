# Network Scanner 🔍

A Python-based network scanning tool for discovering devices on your local network.

## 📋 Overview

Network Scanner is a lightweight Python tool that helps you identify all devices connected to your network. It's perfect for network administrators, security professionals, and anyone wanting to monitor their network activity.

## ✨ Features

- **ARP-based scanning**: Reliable device discovery using ARP requests
- **MAC Address Detection**: Identifies device MAC addresses
- **Vendor Identification**: Shows device manufacturer information
- **IP Range Scanning**: Scan specific IP ranges or entire subnets
- **Clean Output**: Easy-to-read tabular format
- **Cross-platform**: Works on Linux, macOS, and Windows

## 🔧 Prerequisites

- Python 3.6+
- scapy library
- Root/Administrator privileges (required for ARP scanning)

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/0xParth/Network_Scanner.git
cd Network_Scanner

# Install dependencies
pip install -r requirements.txt

# For Linux/Mac users, you might need:
sudo pip install scapy
```

## 🚀 Usage

```bash
# Display help
sudo python network_scanner.py -h

# Scan your local network
sudo python network_scanner.py -t 192.168.1.0/24

# Scan specific IP range
sudo python network_scanner.py -t 192.168.1.1-100

# Scan with verbose output
sudo python network_scanner.py -t 192.168.1.0/24 -v
```

## 📊 Example Output

```
[+] Network Scan Results:
---------------------------------------------------------
IP Address          MAC Address             Vendor
---------------------------------------------------------
192.168.1.1         aa:bb:cc:dd:ee:ff      Cisco Systems
192.168.1.2         11:22:33:44:55:66      Apple Inc.
192.168.1.3         77:88:99:aa:bb:cc      Samsung Electronics
---------------------------------------------------------
[+] Total devices found: 3
```

## ⚙️ Command Line Options

- `-t, --target`: Target IP address or range (required)
- `-v, --verbose`: Enable verbose output
- `-o, --output`: Save results to file
- `-h, --help`: Display help message

## 🛡️ Security Considerations

- This tool requires root/administrator privileges
- Only scan networks you own or have permission to test
- Be aware of your local laws regarding network scanning

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License.

## ⚠️ Disclaimer

This tool is for educational and authorized testing purposes only. Users are responsible for complying with applicable laws. The author is not responsible for misuse or damage caused by this program.

## 👤 About the Author

**0xParth** is a passionate cybersecurity professional who brings together expertise in multiple domains:

- **💻 Security Analyst** - Specializing in vulnerability assessment and security testing
- **🏹 Bug Bounty Hunter** - Active participant in bug bounty programs
- **👨‍💼 Community Leader** - Leading and contributing to the security community
- **📹 YouTuber** - Creating educational content at [@BUGXS](https://youtube.com/@BUGXS)

### Connect with 0xParth:
- **Instagram**: [@0xparth](https://instagram.com/0xparth)
- **LinkedIn**: [/in/parthshu18](https://linkedin.com/in/parthshu18)
- **Twitter**: [@0xparth](https://twitter.com/0xparth)
- **Medium**: [@0xParth](https://medium.com/@0xParth)
- **YouTube**: [@BUGXS](https://youtube.com/@BUGXS)

### Tech Stack:
C, JavaScript, Python, Shell Script, Linux, Jira, Docker, Postman

### Other Projects by 0xParth:
- **[CEH-Practical-Guide](https://github.com/0xParth/CEH-Practical-Guide)** - This Repo will help you to prepare better for CEH - Practical Exam (50 ⭐)
- **[All-Bug-Dorks](https://github.com/0xParth/All-Bug-Dorks)** - Google dorks to find Bug Bounty Programs (1 ⭐)
- **[API_Labs](https://github.com/0xParth/API_Labs)** - Creating API labs for Classes
- **[Network_Scanner](https://github.com/0xParth/Network_Scanner)** - Network scanner utility
- **[MAC_Changer](https://github.com/0xParth/MAC_Changer)** - This script will help you out to change your MAC Address temporarily!
- **[takeoveer](https://github.com/0xParth/takeoveer)** - Subdomain takeover toolkit
- **[0xParth](https://github.com/0xParth/0xParth)** - Config files for my GitHub profile
- **[0xparth.github.io](https://github.com/0xParth/0xparth.github.io)** - Personal website
- **RecIT** - Ultimate Recon Script 💥 (Private)
- **Recon-V2.0** - Backup to /Recon/V2.0 (Private)
- **certsubs-corp** - Certsubs for Enterprise (Private)
- **recon** - Reconnaissance tools (Private)
- **hackathon** - Hackathon projects (Private)
- **certsubs-app** - Certsubs for Bug Bounty Hunters (Private)
- **pyRIT_Wrapper** - PyRIT wrapper utility (Private)
- **allsubz** - All subdomains finder (Private)
- **IntentClassifier** - Intent classification tool (Private)
- **PromptGuard** - Prompt protection utility (Private)
- **DocuCraft-AI** - AI-powered documentation tool (Private)
- **credential-stuffing** - Credential stuffing testing (Private)

## 🙏 Acknowledgments

- Built with Python and Scapy
- Inspired by network discovery needs in bug bounty hunting
