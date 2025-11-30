# 🔱 Instagram Group Renamer 🔱

A powerful, asynchronous Python script designed to continuously and rapidly change the name of an Instagram Direct Message (DM) group chat using the **Playwright** browser automation library. This tool is built for maximum speed and efficiency.

---

## ⚠️ Disclaimer

This script is for **educational and personal use only**. Using automated tools against a platform's terms of service may result in temporary or permanent account suspension. Use at your own risk.

---

## ✨ Features

* **Asynchronous (AsyncIO):** Utilizes Python's `asyncio` for concurrent operations, allowing multiple name change attempts simultaneously.
* **Playwright Integration:** Uses a headless Chromium browser to simulate real user actions, improving reliability.
* **Customizable Names:** Generates unique group names using a customizable prefix, emoji bases, and sequential counters.
* **Live Stats:** Provides real-time success and failure counts directly in the terminal.
* **Session-based:** Authenticates using a `sessionid` cookie, avoiding the need for a username and password login flow.

---

## 🛠️ Prerequisites

Before running the script, ensure you have the following installed:

1.  **Python 3.8+**
2.  **Required Python Libraries:**
    ```bash
    pip install playwright cfonts pyfiglet
    ```
3.  **Playwright Browser Binaries:** The script uses Chromium, so you must install the necessary browser files.
    ```bash
    playwright install chromium
    ```

---

## 🚀 Setup and Execution

### 1. Gather Inputs

You will need three key pieces of information:

| Input | Description |
| :--- | :--- |
| **Script Password** | Hardcoded as `xnsgod`. |
| **Session ID** | Your Instagram `sessionid` cookie value. You must extract this from your browser's Developer Tools (F12) while logged into Instagram. This authenticates your script's actions. |
| **Group Chat URL** | The full URL of the Instagram group chat (e.g., `https://www.instagram.com/direct/t/00000000000000/`). |

### 2. Run the Script

1.  Save the script (e.g., `Renamer.py`) and the optional `ufo_bases.txt` in the same directory.
2.  Execute the script from your terminal:
    ```bash
    python Renamer.py
    ```
3.  Follow the prompts to enter the **password**, **Session ID**, **Group Chat URL**, your **name prefix**, and the desired **number of async tasks**.
