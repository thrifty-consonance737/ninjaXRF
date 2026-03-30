<h1 align="center">⚔️ NinjAXFR v0.1</h1>

<p align="center">
Fast DNS Zone Transfer (AXFR) Scanner for Recon & Security Testing
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-0.1-blue">
  <img src="https://img.shields.io/badge/python-3.x-green">
  <img src="https://img.shields.io/badge/status-active-success">
</p>

---

## 🧠 About

NinjAXFR is a fast and lightweight DNS zone transfer (AXFR) scanner written in Python.
It automates name server discovery and tests for misconfigured DNS servers, helping
identify exposed zone data during reconnaissance and security assessments.

---

## ⚡ Features

- Automatic NS discovery  
- Concurrent scanning  
- AXFR misconfiguration detection  
- Full zone dump (--exploit)  
- Output file support  
- Verbose mode  
- Silent mode  

---

## 📥 Installation

```bash
git clone https://github.com/yHunterDep/ninjaXRF/
cd ninjaxfr
pip install -r requirements.txt
chmod +x ninjaxfr
./ninjaxfr -h
```

---

## 🚀 Usage

```bash
./ninjaxfr -h
```

---

## 📌 Options

```text
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        Target domain to scan
  -xpl, --exploit       Dump full zone data if AXFR is successful.
  -o OUTPUT, --output OUTPUT
                        Save results to a specified file.
  -c CONCURRENT, --concurrent CONCURRENT
                        Number of concurrent threads (default: 25).
  -v, --verbose         Shows detailed information about each step
                        of the scanning process..
  -s, --silent          Skip Banner mode
```

---

## 🧪 Examples

### Single target
```bash
./ninjaxfr -t zonetransfer.me
```

### High concurrency
```bash
./ninjaxfr -t zonetransfer.me -c 70
```

### Multiple domains
```bash
cat domains.txt | ./ninjaxfr
```

### Exploit mode
```bash
./ninjaxfr -t zonetransfer.me --exploit
```

### Save output
```bash
./ninjaxfr -t zonetransfer.me -o results.txt
```

### Pipeline usage
```bash
cat domains.txt | ./ninjaxfr | anew results.txt
```

---

## 🧾 Output Example

```text
Zone Transfer (medium)
Domain: zonetransfer.me
NS_SERVER: nsztm1.digi.ninja
Command to use: dig axfr zonetransfer.me @nsztm1.digi.ninja
```

---

## 🎨 Banner

```text
          _         _      _  __ __________
   ____  (_)___    (_)___ | |/ // ____/ __ \
  / __ \/ / __ \  / / __ `/   // /_  / /_/ /
 / / / / / / / / / / /_/ /   |/ __/ / _, _/
/_/ /_/_/_/ /_/_/ /\__,_/_/|_/_/   /_/ |_|
             /___/

    ninjaXFR - DNS Zone Transfer Tool
    by HunterDep
    v0.1
```

---

## ⚠️ Disclaimer

This tool is intended for educational and authorized security testing purposes only.
Do not use it against targets without permission.

---

## 🧑‍💻 Author

HunterDep

---
