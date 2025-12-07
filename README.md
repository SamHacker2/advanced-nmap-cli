# 📘 Advanced Nmap CLI Toolkit

An advanced Nmap automation script featuring NSE fuzzy search (fzf), NSE debugging, Telegram notifications, full-port scans, OS detection, and an interactive menu designed for ethical hackers and penetration testers.

---

## 🚀 Features

- Interactive menu-based Nmap scanning
- Ping, Quick, Full-Port, OS detection & Aggressive scans
- NSE Script Pattern Matching & Multiple Script Execution
- NSE Debug Mode (deep script trace + logs)
- FZF fuzzy search for NSE scripts
- Automatic intrusion keyword warnings (safe mode)
- Telegram notifications for scan completion
- Automatic output saving (.nmap, .xml, .gnmap)
- Clean error handling and safe execution
- Supports non-interactive automation modes

---

## 📥 Installation

### Clone the repository

This project is licensed under the MIT License.r on GitHub!

```
git clone https://github.com/YOUR-USERNAME/advanced-nmap-cli.git

cd advanced-nmap-cli
```


### Make script executable

```
chmod +x nmap-cli.sh
```

### (Optional) Install globally

```
sudo ./nmap-cli.sh --install
```


## Run using:

```
nmap-cli
```


---

## ⚙️ Configuration (Optional)

### Enable Telegram Alerts

1. Create a bot using @BotFather  
2. Save your BOT_TOKEN  
3. Get your Chat ID using @getidbot  
4. Export variables:

```
echo 'export TELEGRAM_BOT_TOKEN="YOUR_TOKEN"' >> ~/.bashrc
echo 'export TELEGRAM_CHAT_ID="YOUR_CHAT_ID"' >> ~/.bashrc
```


---

## 🖥️ Usage


Menu includes:

- Ping Scan
- Quick Scan
- Full Port Scan
- Service & Version Detection
- OS Detection
- Aggressive Scan
- Specific Port Scan
- NSE Pattern Scan
- NSE Debug
- NSE Fuzzy Search (fzf)

---

## ⚡ Non-Interactive Mode (Automation)

### Quick Scan

```
./nmap-cli.sh -n -t 192.168.1.1 -m quick
```

### Full Port Scan

```
./nmap-cli.sh -n -t scanme.nmap.org -m full
```

### NSE Pattern Scan

```
./nmap-cli.sh -n -t 192.168.1.10 -m nse -a "http*" -p 80,443
```

---

## 🔍 Fuzzy NSE Script Search (fzf)

Fuzzy search NSE scripts:

```
./nmap-cli.sh
```


Select option **11 → NSE Fuzzy Search**

Features:
- Multi-select script picker
- Automatic detection of intrusive scripts
- Saves results automatically

Output saved in:

```
./scans/nse_search/
```


---

## 🐞 NSE Debug Mode

```
./nmap-cli.sh --debug <target> <script-name>
```


Produces:
- Simple NSE execution
- Script trace
- Debug logs
- Output files

---

## 📂 Output Files

All scans are saved to:

```
./scans/
```


Formats:
- .nmap
- .xml
- .gnmap
- Debug trace logs

---

## 🧑‍💻 Author

**Samir Ahamad Khan**  
Ethical Hacker • Security Researcher • Developer

Specialized in:
- Network security
- Nmap automation
- Bash scripting
- Penetration testing

GitHub:  
https://github.com/SamHacker2

---

## ⚠️ Legal Disclaimer

Use this tool only on systems you own or have explicit written permission to test.  
Unauthorized scanning is illegal.  
The author is not responsible for misuse of this tool.

---

## 📜 License

This project is licensed under the **MIT License**.


