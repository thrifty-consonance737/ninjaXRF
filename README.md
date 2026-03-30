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
git clone https://github.com/yourname/ninjaxfr.git
cd ninjaxfr
pip install dnspython
```

---

## 🚀 Usage

```bash
python ninjaxfr.py [options]
```

---

## 📌 Options

```text
-t, --target        Target domain to scan
-c, --concurrent    Number of threads (default: 25)
-xpl, --exploit     Dump full DNS zone if vulnerable
-o, --output        Save results to a file
-v, --verbose       Enable detailed output
-s, --silent        Disable banner
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
