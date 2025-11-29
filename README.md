<p align="center">
  <img src="https://i.imgur.com/tLLNTOv.png" alt="PureCore QRCodefy Logo" width="800">
</p>

<h3 align="center">
  <strong>The only QR Code library you'll ever need.</strong>
</h3>

<p align="center">
  <a href="#-installation">Installation</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-integrations">Integrations</a> •
  <a href="#-api-reference">API</a>
</p>

<p align="center">
  <img src="https://img.shields.io/npm/v/qrcodefy?style=flat-square&color=a855f7" alt="npm version">
  <img src="https://img.shields.io/npm/dm/qrcodefy?style=flat-square&color=3b82f6" alt="downloads">
  <img src="https://img.shields.io/github/license/purecore/qrcodefy?style=flat-square&color=22c55e" alt="license">
</p>

---

## 🎯 Why QRCodefy?

Tired of complex libraries that fail to render in terminal or generate corrupted files?

**QRCodefy solves this.** Designed with Chatbot, Automation, and CLI developers in mind, it bridges the gap between receiving a hash/Base64 and delivering it where you need: on screen or on disk.

<table>
  <tr>
    <td align="center" width="25%">
      <h3>🎯</h3>
      <strong>Base64 & String Focus</strong><br>
      <sub>Perfect for APIs that return QR as text</sub>
    </td>
    <td align="center" width="25%">
      <h3>🖥️</h3>
      <strong>Terminal First</strong><br>
      <sub>Beautiful console rendering (essential for VPS logs)</sub>
    </td>
    <td align="center" width="25%">
      <h3>💾</h3>
      <strong>File System</strong><br>
      <sub>Save to PNG/SVG with one line of code</sub>
    </td>
    <td align="center" width="25%">
      <h3>🤖</h3>
      <strong>Bot Ready</strong><br>
      <sub>Perfect for Baileys, EvolutionAPI & WhatsApp-Web.js</sub>
    </td>
  </tr>
</table>

---

## 📦 Installation

```bash
# npm
npm install qrcodefy

# yarn
yarn add qrcodefy

# bun
bun add qrcodefy
```

---

## 🚀 Quick Start

### CLI Usage

Don't want to write code? Use directly in terminal:

```bash
# Generate in terminal
npx qrcodefy "YourBase64OrTextHere" terminal

# Save to file
npx qrcodefy "YourBase64OrTextHere" ./qrcode.png
```

### Programmatic Usage

```typescript
import { QRCodefy } from 'qrcodefy';

const qr = new QRCodefy('https://example.com');

// Render in terminal
await qr.toTerminal();

// Save to file
await qr.toFile('./qrcode.png');

// Get as Data URL (for HTML <img>)
const dataUrl = await qr.toDataURL();
```

---

## 💡 Integrations

Here's where QRCodefy shines. See how it integrates seamlessly with the most popular WhatsApp libraries.

### 1️⃣ With @whiskeysockets/baileys

Baileys emits a raw connection string. QRCodefy instantly transforms it into a scannable QR in your log.

```typescript
import { makeWASocket, useMultiFileAuthState } from '@whiskeysockets/baileys';
import { QRCodefy } from 'qrcodefy';

async function connectToWhatsApp() {
  const { state, saveCreds } = await useMultiFileAuthState('auth_info_baileys');
  const sock = makeWASocket({ auth: state });

  sock.ev.on('connection.update', async (update) => {
    const { connection, lastDisconnect, qr } = update;

    if (qr) {
      // 🔥 THE MAGIC HAPPENS HERE
      console.log('Scan the QR Code below:');
      const qrcode = new QRCodefy(qr);
      await qrcode.toTerminal(true); // 'true' for compact version
    }

    if (connection === 'close') {
      // Reconnection logic...
    }
  });
}
```

### 2️⃣ With EvolutionAPI (Webhooks)

If you have a backend consuming EvolutionAPI, you often receive the QR Code Base64 via JSON. Use QRCodefy to save it as an image.

```typescript
import express from 'express';
import { QRCodefy } from 'qrcodefy';

const app = express();
app.use(express.json());

app.post('/webhook/evolution', async (req, res) => {
  const { event, data } = req.body;

  if (event === 'qrcode.updated' && data.qrcode) {
    const qrManager = new QRCodefy(data.qrcode);
    
    // Show in server log
    await qrManager.toTerminal();

    // Save to public folder
    await qrManager.toFile('./public/qrcodes/session.png');
    
    console.log('QR Code updated and saved!');
  }
  
  res.sendStatus(200);
});

app.listen(3000);
```

### 3️⃣ With WhatsApp-Web.js

```typescript
import { Client } from 'whatsapp-web.js';
import { QRCodefy } from 'qrcodefy';

const client = new Client();

client.on('qr', async (qr) => {
  console.log('📱 Scan this QR Code:');
  const qrcode = new QRCodefy(qr);
  await qrcode.toTerminal();
  
  // Or save for web interface
  await qrcode.toFile('./public/whatsapp-qr.png');
});

client.initialize();
```

---

## 📚 API Reference

### Constructor

```typescript
new QRCodefy(data: string, options?: QRCodeOptions)
```

Instantiates the class with data (Text, URL, or Base64).

| Parameter | Type | Description |
|-----------|------|-------------|
| `data` | `string` | The content to encode (URL, text, or Base64) |
| `options` | `object` | Optional configuration |

### Methods

#### `toTerminal(small?: boolean): Promise<void>`

Renders the QR Code using ANSI/ASCII characters.

| Parameter | Type | Default | Description |
|-----------|------|---------|-------------|
| `small` | `boolean` | `true` | Use `false` if QR Code is too dense/large |

#### `toFile(path: string): Promise<void>`

Saves the image to disk. Format is detected by extension.

| Parameter | Type | Description |
|-----------|------|-------------|
| `path` | `string` | File path with extension (`.png`, `.svg`) |

#### `toDataURL(): Promise<string>`

Returns the string formatted as `data:image/png;base64,...` ready to be placed in an HTML `<img src="..." />` tag.

---

## 🔧 Configuration Options

```typescript
const qr = new QRCodefy('data', {
  errorCorrectionLevel: 'M', // L, M, Q, H
  margin: 4,
  width: 256,
  color: {
    dark: '#000000',
    light: '#ffffff'
  }
});
```

---

## 📝 License

This project is under the **MIT License**. Feel free to use in your personal and commercial projects.

---

<p align="center">
  Made with 💜 for the Bot Developer Community
</p>

<p align="center">
  <a href="https://github.com/purecore/qrcodefy">⭐ Star us on GitHub</a>
</p>
