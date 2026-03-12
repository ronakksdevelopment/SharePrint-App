🖨️ SharePrint App

SharePrint is a modern, serverless peer-to-peer (P2P) web application designed for fast, seamless document printing across devices. By leveraging WebRTC, SharePrint allows users to connect multiple devices (mobile, tablet, PC) directly to a host computer's printer without needing any backend servers, drivers, or complex network configurations.

When paired with Google Chrome's kiosk printing mode on the host machine, it provides a 100% silent, instant printing experience without any print dialog popups.

🌐 Live Demo

https://ronakksdevelopment.github.io/SharePrint-App/

📦 GitHub Repository

https://github.com/ronakksdevelopment/SharePrint-App

✨ Features

⚡ Serverless P2P Connection: Direct device-to-device file transfer using WebRTC (PeerJS).

📱 Cross-Platform: Works entirely in the browser on mobile, tablet, and desktop.

📷 QR Code Scanning: Instantly connect to a host printer by scanning a QR code.

🖨️ Silent Auto-Printing: Supports 100% silent printing without dialog popups (via Chrome flags).

📄 Format Support: Send PDFs and Images (JPG/PNG) directly to the printer.

🎨 Modern UI: Premium glass-morphism dark theme with intuitive drag-and-drop file selection.

🧠 How It Works

Host Mode: A PC connected to a printer opens the app and starts a "Print Server", generating a unique 5-digit code and QR code.

Client Mode: Any other device enters the code or scans the QR code to establish a secure WebRTC data channel with the Host.

Execution: The client sends a file. The Host receives it, injects it into a hidden iframe, and triggers the browser's native iframe.contentWindow.print() command.

When the Host runs Google Chrome with the --kiosk-printing flag, the browser skips the print dialog and directly sends the document to the default printer.

⚙️ Chrome Kiosk Printing Setup (Windows Host)

To enable automatic silent printing on the Host machine, launch Google Chrome using the following command:

"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk --kiosk-printing [https://ronakksdevelopment.github.io/SharePrint-App/](https://ronakksdevelopment.github.io/SharePrint-App/)


This command will:

Launch Google Chrome in full-screen (Kiosk) mode.

Open the SharePrint App.

Automatically bypass the browser print confirmation dialog.

Print directly to your system's default printer.

🖥️ Create Desktop Shortcut (Recommended)

For quick access on your Host PC:

Right-click on your Desktop.

Select New → Shortcut.

Paste the following target path:

"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk --kiosk-printing [https://ronakksdevelopment.github.io/SharePrint-App/](https://ronakksdevelopment.github.io/SharePrint-App/)


Click Next.

Name the shortcut: SharePrint Server

Click Finish.

Opening this shortcut will launch your Host environment with automatic printing enabled.

🪟 Silent Printing Without Fullscreen

If you want the silent printing capabilities but prefer to keep the standard Chrome window (not full-screen), omit the --kiosk flag:

"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk-printing [https://ronakksdevelopment.github.io/SharePrint-App/](https://ronakksdevelopment.github.io/SharePrint-App/)


🖨️ Set Default Printer

Before starting your SharePrint Host session:

Open Google Chrome.

Press Ctrl + P to open the standard print dialog.

Select your preferred physical printer from the destination dropdown.

Cancel the print job.
(Chrome remembers the last used printer and treats it as the default for kiosk mode).

⌨️ Exit Kiosk Mode

To close Kiosk mode on the Host machine, press:
Alt + F4

💡 Use Cases

Office Printing Dashboards: Allow anyone in the office to print without installing drivers.

Cyber Café Printing Stations: Let customers print directly from their phones.

POS Receipt Printing: Send receipts from a mobile tablet to a central printer.

Self-Service Printing: Fast, automated document retrieval.

📄 License

This project is open-source and available for educational, practical, and commercial use.

⭐ If you find this project useful, consider giving it a star on GitHub!
