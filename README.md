# 🐺 Wolf Pass Generator v3.1  
### Advanced Multi-Mode Password Generation Tool  
**Developed by Wolf Security Team**

---

## 🧩 Overview

**Wolf Pass Generator** is a powerful and flexible Python tool that generates password lists for penetration testing, cybersecurity research, and advanced security analysis.  
It offers multiple generation algorithms — including random, victim-based, hybrid, and combinator patterns — capable of producing up to **30 million passwords**.

---

## ⚡ Features

- 🔢 **Random password generation** using multiple formats (alpha, numeric, special, etc.)
- 👤 **Victim-based generation** using user-defined info (name, year, keywords, etc.)
- 💡 **6 smart algorithms** (`basic`, `leet`, `advanced`, `combinator`, `massive`, `hybrid`)
- 💾 **Supports loading `rockyou.txt`** for common password analysis
- 🧠 **Custom format parsing** (`"word"numbspecial`)
- 🧮 **High performance** — handles millions of passwords efficiently
- 🌈 **Beautiful terminal colors & banners**
- 🧰 **Interactive mode + Command-line mode**

---

## 🛠️ Installation

### Requirements
Make sure you have **Python 3.7+** installed.

```bash
python --version
```

### Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/Wolf-Pass-Generator.git
cd Wolf-Pass-Generator
```

### Run the Tool
```bash
python wolf_pass_generator.py
```

---

## 🧠 Usage

### Command-Line Examples

#### 🔹 Random Password Generation
```bash
python wolf_pass_generator.py -g -f all -l 12 -c 100
```

#### 🔹 Victim-Based Generation
```bash
python wolf_pass_generator.py -v -a massive,hybrid -c 50000 -n victim_list.txt
```

#### 🔹 Load RockYou List
```bash
python wolf_pass_generator.py -r -c 100000 -n rockyou_filtered.txt
```

#### 🔹 Interactive Mode
```bash
python wolf_pass_generator.py
```

---

## 🧩 Format Types

| Type | Description |
|------|--------------|
| `bigalpha` | Uppercase letters (A–Z) |
| `smallalpha` | Lowercase letters (a–z) |
| `alpha` | Both upper and lower case |
| `numeric` | Numbers (0–9) |
| `special` | Special characters |
| `alphanumeric` | Letters + numbers |
| `all` | All character types combined |
| `custom` | User-defined patterns |

**Custom format examples:**
```bash
"word"numb
bigalphasmallalphanumb
alpha"123"special
```

---

## 🧠 Algorithms Overview

| Algorithm | Description |
|------------|-------------|
| `basic` | Basic combinations with special chars and years |
| `leet` | Converts letters into leet-style numbers |
| `advanced` | Adds suffixes and complex combinations |
| `combinator` | Merges multiple victim keywords |
| `massive` | Generates extensive variations |
| `hybrid` | Combines multiple transformation techniques |

---

## 💾 Output

All generated passwords can be automatically saved to a file:
```bash
python wolf_pass_generator.py -g -f alpha -l 10 -c 50 -n output.txt
```

Example output file (`output.txt`):
```
Alpha2025!
aLph@123
ALPHA!2024
...
```

---

## ⚠️ Legal Disclaimer

This project is created **strictly for educational and cybersecurity research purposes**.  
Do **not** use this tool for unauthorized attacks or any illegal activities.  
The author(s) are **not responsible** for any misuse or damage caused by this software.

---

## 🐺 Credits

- **Developer:** Wolf Security Team  
- **Version:** 3.1  
- **Languages:** Python 3  
- **Banner:** Custom ANSI Art  

---

## 📜 License

This project is released under the **MIT License** — free to modify and distribute with attribution.

---

> 🧠 *"Strong passwords protect weak systems. Weak passwords destroy strong systems."*  
> — Wolf Security Team
