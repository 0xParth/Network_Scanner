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

## 👤 Author

**0xParth**
- GitHub: [@0xParth](https://github.com/0xParth)
- Twitter: [@0xparth](https://twitter.com/0xparth)

## 🙏 Acknowledgments

- Built with Python and Scapy
- Inspired by network discovery needs in bug bounty hunting
