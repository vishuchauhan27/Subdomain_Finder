# 🔍 Subdomain Enumeration and Vulnerability Scanning Script

This is a comprehensive bash script designed for subdomain enumeration, DNS resolution, live host detection, and vulnerability scanning. It integrates several popular tools to automate recon tasks and streamline the discovery of potentially vulnerable targets in a domain.

## ⚙️ Features
- **Subdomain Enumeration** using multiple tools: `subfinder`, `amass`, `assetfinder`, `findomain`, `waybackurls`, `shuffledns`, and CRT.SH scraping.
- **DNS Resolution** with `MassDNS` and `DNSx`.
- **Live Host Detection** using `httprobe` and `naabu`.
- **Screenshot Capture** with `Aquatone` and `Gowitness`.
- **Port Scanning** with `Nmap` (Basic and High modes).
- **Vulnerability Scanning** with `Nuclei`, `Nikto`, `Gf`, and `ffuf`.

## 🚀 How to Use

### 📥 Installation
Ensure you have the required tools installed on your system:
- `subfinder`, `amass`, `assetfinder`, `findomain`, `waybackurls`, `shuffledns`, `curl`, `jq`
- `MassDNS`, `DNSx`, `httprobe`, `naabu`, `Aquatone`, `Gowitness`
- `Nmap`, `Nuclei`, `Nikto`, `Gf`, `ffuf`

### 📜 Usage
Run the script with the domain and scan mode as arguments:

```bash
./scan.sh <domain> <scan_mode>
```
### Parameters:

- <domain>: The target domain to discover subdomains for.
- <scan_mode>: Choose between basic (Top 1000 ports scan) or high (Full port scan with OS and service detection).

### Example :
```bash
./scan.sh example.com <low or high>
```

