

# 🌙 lunofetch

A **lightweight, modern, and customizable Neofetch alternative** written in Python.  
It displays essential **system information** with your own **ASCII logo**, and works on any Linux distribution.

---

##  Features

-  Custom ASCII logo support (`--logo` option)
-  Minimal dependencies (`psutil`, `distro`)
-  Colored terminal output (auto-detects TTY)
-  Works on **Arch, Ubuntu, Fedora, Debian, and any POSIX system**
-  Human-readable system stats (uptime, memory, disk, CPU)
-  Single Python script — fast and clean

---

##  Installation

You can install directly from **PyPI**:

```bash
pip install lunofetch
````

Or install locally from source:

```bash
git clone https://github.com/tharunbala/lunofetch.git
cd lunofetch
pip install .
```

---

##  Usage

Once installed, simply run:

```bash
lunofetch
```

### 🔧 Optional Arguments

| Argument        | Description                      |
| --------------- | -------------------------------- |
| `--logo <path>` | Specify a custom ASCII logo file |
| `--no-color`    | Disable colored output           |

---

## 🧩 Example Output

```bash
                                                                    OS: Arch Linux
                                                                   Host: NoMoreMercy
                                                                   Kernel: #1 SMP PREEMPT_DYNAMIC Thu, 02 Oct 2025 19:26:36 +0000
                                                                   Uptime: 0:32:38
                                                                   CPU: AMD Rygen 5 7235HS (8 cores)
                                                                   Memory: 3.0GB/23.2GB (13.0%)
                                                                   Disk: 46.9GB/475.9GB
                              :-==-.                               Shell: /bin/zsh
                        .+@@@@@%+-.                                Terminal: tmux-256color
                      +@@@@@#.
                    *@@@@@*
                  -@@@@@@:
                 +@@@@@%.
                :@@@@@@.
               .@@@@@@*  ==
               =@@@@@@-  #@+
               *@@@@@*  *@@@@@%*-
               #@@@. =@@@@@@@@:
               +@@@%+.   =@@#
               =@@@@@@@#  .@-
                @@@@@@@@%  .                    :
                 %@@@@@@@@:                   .%.
                 .@@@@@@@@@@=               :%%
                   *@@@@@@@@@@%*:       .+%@@+
                    .*@@@@@@@@@@@@@@@@@@@@@#.
                       =%@@@@@@@@@@@@@@@%=
                           =*#@@@@@#*=.







```

---

## 🖼️ Screenshots

| Screenshot | Description |
|-------------|--------------|
| ![Screenshot 1](screenshots/Screenshot%201.png) | Default `lunofetch` output with embedded ASCII logo |
| ![Screenshot 2](screenshots/Screenshot%202.png) | Custom logo example with `--logo mylogo.txt` |
| ![Screenshot 3](screenshots/Screenshot%203.png) | Output without colors (`--no-color`) |

*(Ensure your screenshots are stored in a folder named `/screenshots` in your repository root.)*


##  How It Works

`lunofetch` gathers system information using Python’s built-in modules and optional dependencies:

* `platform` — for OS, kernel, and host details
* `psutil` — for memory, uptime, and CPU stats
* `shutil` — for disk usage
* `distro` — for Linux distribution info

It then formats and aligns the ASCII art with system information for a clean terminal display.

---

##  Developer Usage

Run from source for development:

```bash
python3 -m lunofetch
```

To specify a logo:

```bash
python3 -m lunofetch --logo ascii/arch.txt
```

---

##  Project Structure

```
lunofetch/
├── lunofetch/
│   └── __init__.py
├── README.md
├── LICENSE
├── pyproject.toml
├── setup.cfg
└── screenshots/
    ├── screen1.png
    ├── screen2.png
    └── screen3.png
```

---

##  License

This project is licensed under the **MIT License**.
See the [LICENSE](LICENSE) file for details.

---

##  Author

**B. Tharun Bala**
📧 `balat4880@gmail.com`
🎓 B.Tech Artificial Intelligence and Data Science
ER. Perumal Manimekalai College of Engineering, Hosur

---

##  Contributing

Pull requests are welcome!
If you’d like to add features (like GPU info, package count, or distro logos), fork the repo and open a PR.

---

##  Requirements

* Python 3.7+
* Optional: `psutil`, `distro`

Install dependencies manually if not auto-installed:

```bash
pip install psutil distro
```

---

##  Example Custom Logo

```bash
lunofetch --logo ~/logos/arch.txt
```

Example logo file (`arch.txt`):

```
      /\
     /  \    OS: Arch Linux
    / /\ \   CPU: Ryzen 7
   / ____ \
  /_/    \_\
```

---

##  Links

* 📦 PyPI: [https://pypi.org/project/lunofetch](https://pypi.org/project/lunofetch/)
* 💻 GitHub: [https://github.com/Hackb07/lunofetch](https://github.com/Hackb07/lunofetch)

---

> 💬 *“Lunofetch — because your terminal deserves to look beautiful.”*

```

