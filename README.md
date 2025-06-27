# 🛡️ Custom Rules for Nemesida WAF Enterprise and Community Edition

A collection of custom rules for [Nemesida WAF](https://www.nemesida-waf.com/), designed to enhance detection and protection against specific web threats and tailored attack patterns.

---

## 📄 Table of Contents
- [About](#about)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## 📌 About

This repository contains custom rules I've developed to extend the capabilities of **Nemesida WAF** beyond its default signatures. These rules address specific use cases, niche attack vectors, or edge-case traffic patterns that are not sufficiently covered by standard rulesets. Please note that these rules will be updated and tweaked.

Tested with:
- Wordpress
- WinterCMS
- OctoberCMS
- EspoCRM
- Codeigniter 3 and 4

---

## ✨ Features

- Covers edge-case SQLi, XSS, and RCE patterns
- Fine-tuned to reduce false positives
- Easy to integrate with existing Nemesida WAF setups
- Annotated for clarity and customization

---

## 🔧 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/novastream/NWafRules.git
   ```
2. Copy the rules into Nemesida WAF configuration file:
   ```bash
   sudo nano /etc/nginx/nwaf/conf/global/nwaf.conf
   ```

3. Reload your web server:
   ```bash
   systemctl reload nginx
   ```

---

## 🚀 Usage

After integration, Nemesida WAF will automatically apply these rules to incoming traffic. Monitor logs at `/var/log/nginx/error.log` to verify detections.

You can test the rules using standard web vulnerability scanners or manual requests.

Just add a hashtag in front of the rule to disable it.

---

## 🤝 Contributing

Contributions, suggestions, and issue reports are welcome!

1. Fork this repo
2. Create a new branch
3. Add or modify rules
4. Submit a pull request with a description of the change

---

## 📜 License

This project is licensed under the MIT License.