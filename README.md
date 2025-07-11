# 🔐 FingerPrintica

**FingerPrintica** is a simple, static web app that demonstrates how to use built-in biometric fingerprint authentication using the WebAuthn API. It works on devices with platform authenticators such as fingerprint sensors, Face ID, or Windows Hello.

> 💡 Requires HTTPS and a supported browser.

---

## 🌟 Features

- Register with biometric fingerprint or other platform authenticator
- Authenticate with a single touch
- Stores credential ID securely in local storage (for demo purposes)
- Uses native WebAuthn API (no third-party libraries)

---

## 🚀 Demo

You can try the live demo here:  
👉 [https://your-demo-link.com](https://your-demo-link.com) *(replace with actual URL)*

---

## 🖥️ Requirements

- A device with a biometric sensor (fingerprint, Face ID, Windows Hello)
- Modern browser (Chrome, Edge, Safari, Firefox)
- HTTPS environment

> ⚠️ WebAuthn requires a secure context (HTTPS or `localhost`).

---

## 📁 Files

- `index.html` – Main static page with biometric registration and login
- No backend required — 100% static and client-side

---

## 🛠️ How to Use Locally

1. Clone or download the repository.
2. Serve the `index.html` file over HTTPS (required for WebAuthn).

```bash
# Install http-server globally if not already
npm install -g http-server

# Generate SSL certs with mkcert (https://github.com/FiloSottile/mkcert)
mkcert localhost

# Start server with HTTPS
http-server -S -C localhost.pem -K localhost-key.pem
