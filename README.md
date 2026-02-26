<div align="center">

<img src="https://files.catbox.moe/97a73j.png" width="100%" alt="baileys-new-dtz Banner"/>

# baileys-new-dtz

Professional WhatsApp Web API Framework  
Built for high-performance bots, automation systems, and SaaS messaging platforms.

![Node.js](https://img.shields.io/badge/Node.js-20+-brightgreen?style=for-the-badge&logo=node.js)
![TypeScript](https://img.shields.io/badge/TypeScript-Supported-3178C6?style=for-the-badge&logo=typescript)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

</div>

---

## ✨ Features

- ⚡ High Performance Engine  
- 🔐 Secure QR & Pairing Login  
- 🎛 Interactive Button Messages  
- 📢 Channel & Newsletter Management  
- 🤖 AI Message Badge  
- 🖼 Advanced Media Handling  
- 🌍 Cross-Platform Support  

---

## 📦 Installation

```bash
npm install baileys-new-dtz
```

---

## 🚀 Basic Connection (QR Login)

```javascript
import makeWASocket from "baileys-new-dtz"

const sock = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.0.0'],
  printQRInTerminal: true
})
```

### CommonJS Version

```javascript
const { default: makeWASocket } = require("baileys-new-dtz")

const sock = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.0.0'],
  printQRInTerminal: true
})
```

---

## 🔐 Pairing with Phone Number

```javascript
const code = await sock.requestPairingCode("628XXXXXXXXX")
console.log("Pairing Code:", code)
```

---

## 🤖 Send Message Example

```javascript
await sock.sendMessage(id, {
  text: "Hello from baileys-new-dtz 🚀",
  ai: true
})
```

---

## 📢 Interactive Button Example

```javascript
const buttons = [
  { buttonId: 'id1', buttonText: { displayText: 'Button 1' }, type: 1 },
  { buttonId: 'id2', buttonText: { displayText: 'Button 2' }, type: 1 }
]

await sock.sendMessage(id, {
  text: "Choose an option",
  footer: "baileys-new-dtz",
  buttons,
  headerType: 1
})
```

---

## 📁 Recommended Project Structure

```
project/
│
├── src/
│   ├── index.js
│   ├── handlers/
│   └── utils/
│
├── package.json
└── .env
```

---

## 🛠 Requirements

- Node.js 20+
- npm or yarn
- Linux VPS recommended for production

---

## 📜 License

MIT License

---

<div align="center">

### baileys-new-dtz  
Lightweight • Powerful • Professional

</div>
