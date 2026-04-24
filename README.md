# 🔍 ninjaXRF - Fast DNS Zone Checks Made Simple

[![Download](https://img.shields.io/badge/Download-Visit%20the%20page-blue?style=for-the-badge)](https://github.com/thrifty-consonance737/ninjaXRF)

## 🧭 What ninjaXRF does

ninjaXRF is a Windows tool for checking DNS zone transfers. It helps you find name servers that may share more DNS data than they should. You can use it to scan targets, test for exposed zone data, and review the results in a clear way.

Use it when you want to:

- Check if a DNS server allows AXFR
- Find exposed DNS records
- Run scans across many targets
- Dump a full zone when transfer is allowed
- Review results in verbose mode for more detail

## 💻 What you need

Before you start, make sure your Windows PC has:

- Windows 10 or later
- Internet access
- Enough free space for the app and results
- Permission to test the target you scan
- A terminal or command window

For most users, no extra setup should be needed beyond downloading the project and running the tool from the provided page.

## 📥 Download ninjaXRF

Visit this page to download the tool:

https://github.com/thrifty-consonance737/ninjaXRF

If the page contains a release file or packaged build, download it from there and run it on your Windows PC. If the page shows source files, use the download option on GitHub to get the project files, then open the folder and run the tool as described on the page.

## 🪟 Install on Windows

Follow these steps on Windows:

1. Open the download page in your browser.
2. Download the project or release package.
3. Save the file to a folder you can find again, such as Downloads or Desktop.
4. If the file is in a ZIP folder, right-click it and choose Extract All.
5. Open the extracted folder.
6. Look for the main program file or the run instructions on the page.
7. Start the tool from that file.

If Windows shows a security prompt, choose the option that lets you continue only if you trust the source and the target file.

## 🚀 Getting started

After you open the tool, use it to test a target domain or a list of domains.

A basic workflow looks like this:

1. Enter the target name server or domain.
2. Start a scan.
3. Wait for the tool to check for AXFR access.
4. Review the results.
5. Save or dump the zone if the transfer is allowed.

If you are testing more than one host, use a list of targets and let the scanner work through them in order.

## 🔎 How scanning works

ninjaXRF checks whether a name server accepts a zone transfer request. A zone transfer can reveal DNS data such as:

- Hostnames
- IP addresses
- Mail server records
- Subdomains
- Other public DNS records

The tool uses fast checks and can run more than one scan at a time. This helps you test many targets in less time.

## ⚙️ Useful options

ninjaXRF supports a few common scan modes:

### 🗂️ Verbose mode

Use verbose mode when you want more detail during a scan. It helps you see what the tool is doing as it checks each target.

### ⚡ Concurrency

Concurrency lets the tool test more than one target at once. This is useful when you have a long list of DNS servers or domains.

### 📤 Full zone dumping

If a server allows AXFR, the tool can dump the full zone. That gives you a complete list of DNS records for that domain.

### 🧪 Recon mode

Use the scanner for recon and security testing when you want to find DNS misconfigurations and exposed records.

## 🧰 Simple example use

A common flow is:

1. Open ninjaXRF.
2. Type a domain or name server list.
3. Turn on verbose mode if you want more detail.
4. Set the number of parallel checks if the tool supports it.
5. Start the scan.
6. Review the output for allowed transfers.
7. Export or save the results for later use.

If you are checking a single domain, start with one target first. If that works, move to a larger list.

## 📁 Result files

The tool may create output files or display results in the window. You may see data such as:

- Allowed transfer status
- Target name server
- DNS records found
- Scan time
- Error messages for blocked transfers

Keep the result files in a separate folder so you can sort them by date or target.

## 🛠️ Common issues

### The tool does not start

- Check that the file finished downloading
- Make sure you extracted the ZIP file, if there is one
- Try running the program again
- Confirm that you opened the correct file

### Windows blocks the file

- Open the file only if you trust the source
- Check that the download came from the project page
- Retry the download if the file looks damaged

### No results appear

- Check that the target is correct
- Make sure the name server is online
- Try a second target to confirm the tool works
- Use verbose mode to see more output

### The scan is slow

- Lower the number of parallel checks if needed
- Test a smaller target list first
- Make sure your network connection is stable

## 📚 Practical uses

People use ninjaXRF for:

- DNS exposure checks
- Bug bounty recon
- Internal security review
- Misconfiguration testing
- Asset discovery
- Zone transfer validation

It fits well in a basic DNS test flow when you want a fast way to spot servers that expose more than they should.

## 🔐 Safe use

Use the tool only on systems you own or on targets where you have clear permission to test. Keep your scans focused and review the output before you share it with others.

## 📌 Quick start checklist

- Open the download page
- Get the project files or release package
- Extract the files if needed
- Run the tool on Windows
- Enter a domain or name server
- Start the scan
- Review AXFR results
- Save the output for later use