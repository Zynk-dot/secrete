# Private Browser

**Private Browser** is a lightweight web tool that allows users to open websites inside a stealth iframe using a CORS proxy, with no history stored and minimal tracking.  
Built for quick, private access to webpages without leaving a trace in your local browser history.

---

## 🚀 Features

-  **Stealth Tab Loading**  
  Opens any URL inside a dynamically generated new tab.
  
-  **No Browsing History**  
  Pages are loaded within an isolated environment using a proxy, avoiding direct local history logging.

-  **Dynamic Navigation**  
  Clicked links inside the page will automatically be reloaded stealthily inside the same frame.

-  **Copy URL Helper**  
  If a page fails to load, users can easily copy the intended URL.

-  **No Installation Required**  
  100% browser-based, simple HTML + JavaScript.

---

## 📸 Screenshot

<!-- Optional: Add an image here -->
<!-- ![Screenshot](screenshot.png) -->

---

## 📖 How It Works

1. **User** enters a URL in the input field and clicks **Go**.
2. **JavaScript** checks if the URL starts with `http` and corrects it if needed.
3. A **new blank tab** is opened (`about:blank`).
4. The stealth tab loads a dynamic HTML page that:
   - Uses the **[AllOrigins](https://allorigins.win/)** public proxy to bypass CORS restrictions.
   - Embeds the page contents inside an `<iframe>`.
   - Handles **internal navigation** by intercepting `<a>` tag clicks.
5. If the proxy fails, the tool gracefully shows a **manual copyable link**.

---

## ⚠️ Warnings

- **Not all websites** will load correctly (especially if they use CSP (Content-Security-Policy) headers or advanced anti-iframe protection).
- **Proxy usage** is reliant on external services like [AllOrigins API](https://allorigins.win/).
- **JavaScript execution** might be limited inside the proxy depending on the website.

---

## 🔧 Installation

No installation needed!

Just open the HTML file (`index.html`) in any modern web browser (Chrome, Firefox, Edge).

If you want to self-host:
```bash
git clone https://github.com/Zynk-dot/secrete.git
cd secrete
# open index.html in browser
```

---

## 🛡️ Disclaimer

This tool is intended for educational and personal use.  
**Do not** use it for unauthorized access or to bypass paywalls, login pages, or private content.  
Always respect website terms of service and laws in your country.

---

## 🙌 Credits

- Developed by [**Zynk-dot**](https://github.com/Zynk-dot)
- Powered by [AllOrigins CORS Proxy](https://allorigins.win/)

---

## 📄 License

This project is open-source under the **MIT License**.  
See [LICENSE](LICENSE) for details.
