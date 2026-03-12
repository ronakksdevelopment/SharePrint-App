````markdown
# 🖨️ SharePrint App

SharePrint App is a **simple browser-based printing utility** designed for **fast and automatic document printing directly from a web interface**. It is useful for environments where quick printing is required without repeatedly opening the print dialog.

The project works best with **Google Chrome kiosk printing mode**, allowing documents to print instantly to the default printer.

---

## 🌐 Live Demo

https://ronakksdevelopment.github.io/SharePrint-App/

---

## 📦 GitHub Repository

https://github.com/ronakksdevelopment/SharePrint-App

---

## ✨ Features

- ⚡ Fast browser-based printing
- 🖨️ Automatic printing support
- 🚫 No print dialog popup (silent printing)
- 🧾 Instant document printing
- 💻 Works with Google Chrome
- 🔧 Easy setup and usage
- 🌐 Runs directly from the browser

---

## 🧠 How It Works

The application triggers printing using the browser’s built-in JavaScript function:

```javascript
window.print();
````

When **Google Chrome** is launched with the `--kiosk-printing` flag, the browser **skips the print dialog** and directly sends the document to the **default printer**.

---

## ⚙️ Chrome Kiosk Printing Setup (Windows)

To enable **automatic silent printing**, launch Google Chrome using the following command:

```
"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk --kiosk-printing https://ronakksdevelopment.github.io/SharePrint-App/
```

This command will:

* Launch Google Chrome
* Open the SharePrint App
* Enable kiosk mode
* Enable silent printing
* Print directly to the default printer

---

## 🖥️ Create Desktop Shortcut (Recommended)

1. Right-click on the **Desktop**
2. Select **New → Shortcut**
3. Paste the following command:

```
"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk --kiosk-printing https://ronakksdevelopment.github.io/SharePrint-App/
```

4. Click **Next**
5. Name the shortcut:

```
SharePrint Kiosk
```

6. Click **Finish**

Opening this shortcut will launch Chrome with **automatic printing enabled**.

---

## 🪟 Silent Printing Without Fullscreen

If you do not want fullscreen kiosk mode, use:

```
"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk-printing https://ronakksdevelopment.github.io/SharePrint-App/
```

This keeps the normal Chrome window but still enables **silent printing**.

---

## 🖨️ Set Default Printer

Before using kiosk printing:

1. Open **Google Chrome**
2. Press **Ctrl + P**
3. Select your preferred printer
4. Set it as the **default printer**

Chrome will automatically send print jobs to this printer.

---

## ⌨️ Exit Kiosk Mode

To close kiosk mode press:

```
Alt + F4
```

---

## 💡 Use Cases

* Print kiosks
* Cyber café printing stations
* POS receipt printing
* Automated document printing
* Self-service printing systems
* Office printing dashboards

---

## 📄 License

This project is open-source and available for educational and practical use.

---

⭐ If you find this project useful, consider **starring the repository**.

```
```
