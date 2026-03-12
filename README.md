<div align="center">
<img src="https://cdn.iconscout.com/icon/free/png-512/free-printer-icon-svg-download-png-1093488.png?f=webp&w=256" alt="SharePrint Logo" width="120" />
<h1>🖨️ SharePrint App</h1>
<p><strong>A secure, serverless P2P printing utility for fast and automatic document printing.</strong></p>

</div>

SharePrint is a browser-based peer-to-peer (P2P) web application designed to link mobile devices or secondary computers directly to a primary print server without requiring a backend. It is especially powerful when paired with Google Chrome's kiosk printing mode, allowing documents to print instantly without repeatedly opening the print dialog window.

✨ Features

⚡ Fast & Direct: Peer-to-Peer (WebRTC) file transfer. No files are stored on external servers.

🖨️ Automatic Printing: Supports bypassing the print dialog for 100% silent printing.

🧾 Instant Document Transfer: Send PDFs and images directly to the host printer.

💻 Cross-Platform: Works seamlessly across PC, tablet, and mobile browsers.

🔧 Zero Setup: Runs completely in the browser with no installation required.

🧠 How It Works

Host opens the app on a PC connected to a printer and generates a 5-digit room code.

Client (mobile or another PC) joins the room using the code or QR scanner.

Client selects a document and sends it directly over a secure P2P connection.

Host receives the file and triggers the browser's built-in window.print() function to physically print the document.

⚙️ Chrome Kiosk Printing Setup (Windows)

To enable automatic silent printing (skipping the print preview dialog), you must launch Google Chrome on the Host PC with specific flags.

1. Set Your Default Printer

Before using kiosk printing:

Open Google Chrome.

Press Ctrl + P to open the print dialog.

Select your preferred physical printer.

Set it as the default printer in your Windows/OS settings.

2. Create a Desktop Shortcut (Recommended)

Right-click on your Desktop and select New → Shortcut.

Paste the following exact command into the location box:

"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk --kiosk-printing [https://ronakksdevelopment.github.io/SharePrint-App/](https://ronakksdevelopment.github.io/SharePrint-App/)


Click Next.

Name the shortcut something recognizable, like SharePrint Kiosk.

Click Finish.

Opening this shortcut will launch Chrome in fullscreen with automatic silent printing enabled. (To exit this fullscreen mode, simply press Alt + F4).

🪟 Silent Printing Without Fullscreen

If you want silent printing but prefer to keep the normal windowed Chrome interface, use this command instead:

"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk-printing [https://ronakksdevelopment.github.io/SharePrint-App/](https://ronakksdevelopment.github.io/SharePrint-App/)


💡 Use Cases

Print Kiosks: Setup a dedicated iPad or tablet next to a PC for customers to print.

Cyber Café Stations: Allow users to print directly from their phones to a master printer.

POS Receipt Printing: Send receipts from a mobile ordering device to a central counter printer.

Office Dashboards: Quick, frictionless printing without installing network drivers on every employee's phone.

📄 License

This project is open-source and available for educational and practical use.

<div align="center">





⭐ <i>If you find this project useful, consider <b>starring the repository!</b></i> ⭐
</div>
