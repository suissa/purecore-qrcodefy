<div style="width: 100%; max-width: 900px; margin: 0 auto; padding: 20px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%); color: #f5f5f5; border-radius: 16px; box-shadow: 0 20px 40px rgba(0,0,0,0.3);">
  
  <!-- Header Section -->
  <div style="text-align: center; padding: 40px 20px; border-bottom: 1px solid #333;">
    <img src="https://i.imgur.com/Tr5F6XV.png" alt="PureCore Logo" style="width: min(300px, 60%); margin-bottom: 20px;">
    <img src="https://i.imgur.com/yh8Aqev.png" alt="QRCodefy Logo" style="width: min(250px, 50%); margin-top: -30px;">
    <h1 style="font-size: 2.5rem; font-weight: 700; margin: 20px 0; background: linear-gradient(135deg, #a855f7, #3b82f6); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">📱 QRCodefy</h1>
    <p style="font-size: 1.2rem; color: #eab308; margin: 10px 0; font-weight: 600;">The only QR Code library you'll ever need.</p>
    
  <div style="display: flex; justify-content: center; gap: 10px; flex-wrap: wrap; margin-top: 30px;">
      <a href="#installation" style="color: #a0a0a0; text-decoration: none; padding: 8px 16px; border: 1px solid #333; border-radius: 20px; font-size: 0.9rem; transition: all 0.2s;">📦 Installation</a>
      <a href="#quick-start" style="color: #a0a0a0; text-decoration: none; padding: 8px 16px; border: 1px solid #333; border-radius: 20px; font-size: 0.9rem; transition: all 0.2s;">🚀 Quick Start</a>
      <a href="#integrations" style="color: #a0a0a0; text-decoration: none; padding: 8px 16px; border: 1px solid #333; border-radius: 20px; font-size: 0.9rem; transition: all 0.2s;">💡 Integrations</a>
      <a href="#api" style="color: #a0a0a0; text-decoration: none; padding: 8px 16px; border: 1px solid #333; border-radius: 20px; font-size: 0.9rem; transition: all 0.2s;">📚 API</a>
    </div>
  </div>

  <!-- Why QRCodefy Section -->
  <div style="padding: 40px 20px; text-align: center; border-bottom: 1px solid #333;">
    <h2 style="font-size: 2rem; margin-bottom: 20px; display: flex; align-items: center; justify-content: center; gap: 10px;">🎯 Why QRCodefy?</h2>
    <p style="color: #a0a0a0; margin-bottom: 10px; line-height: 1.6;">Tired of complex libraries that fail to render in terminal or generate corrupted files?</p>
    <p style="color: #f5f5f5; font-weight: 600; margin-bottom: 30px;"><strong>QRCodefy solves this.</strong> Designed with Chatbot, Automation, and CLI developers in mind, it bridges the gap between receiving a hash/Base64 and delivering it where you need: on screen or on disk.</p>
    
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin-top: 30px;">
      <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; transition: all 0.2s;">
        <div style="font-size: 2rem; margin-bottom: 10px;">🎯</div>
        <h4 style="color: #f5f5f5; margin: 0 0 10px; font-family: 'Inter', sans-serif;">Base64 & String Focus</h4>
        <p style="color: #666; margin: 0; font-size: 0.9rem;">Perfect for APIs that return QR as text</p>
      </div>
      <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; transition: all 0.2s;">
        <div style="font-size: 2rem; margin-bottom: 10px;">🖥️</div>
        <h4 style="color: #f5f5f5; margin: 0 0 10px; font-family: 'Inter', sans-serif;">Terminal First</h4>
        <p style="color: #666; margin: 0; font-size: 0.9rem;">Beautiful console rendering (essential for VPS server logs)</p>
      </div>
      <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; transition: all 0.2s;">
        <div style="font-size: 2rem; margin-bottom: 10px;">💾</div>
        <h4 style="color: #f5f5f5; margin: 0 0 10px; font-family: 'Inter', sans-serif;">File System</h4>
        <p style="color: #666; margin: 0; font-size: 0.9rem;">Save to PNG/SVG with one line of code</p>
      </div>
      <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; transition: all 0.2s;">
        <div style="font-size: 2rem; margin-bottom: 10px;">🤖</div>
        <h4 style="color: #f5f5f5; margin: 0 0 10px; font-family: 'Inter', sans-serif;">Bot Ready</h4>
        <p style="color: #666; margin: 0; font-size: 0.9rem;">Perfect companion for Baileys, EvolutionAPI and WhatsApp-Web.js</p>
      </div>
    </div>
  </div>

  <!-- Installation Section -->
  <div id="installation" style="padding: 40px 20px; border-bottom: 1px solid #333;">
    <h2 style="font-size: 2rem; margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">📦 Installation</h2>
    <pre style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; overflow-x: auto; margin: 20px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.9rem; color: #a0a0a0;"># npm
npm install qrcodefy

# yarn
yarn add qrcodefy

# bun
bun add qrcodefy</code></pre>
  </div>

  <!-- Quick Start Section -->
  <div id="quick-start" style="padding: 40px 20px; border-bottom: 1px solid #333;">
    <h2 style="font-size: 2rem; margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">🚀 Quick Start</h2>
    
  <h3 style="font-size: 1.5rem; margin: 30px 0 15px; color: #3b82f6;">CLI Usage</h3>
    <p style="color: #a0a0a0; margin-bottom: 20px;">Don't want to write code? Use directly in terminal:</p>
    <pre style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; overflow-x: auto; margin: 20px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.9rem; color: #a0a0a0;"># Generate in terminal
npx qrcodefy "YourBase64OrTextHere" terminal

# Save to file
npx qrcodefy "YourBase64OrTextHere" ./qrcode.png</code></pre>

  <h3 style="font-size: 1.5rem; margin: 30px 0 15px; color: #3b82f6;">Programmatic Usage</h3>
    <pre style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; overflow-x: auto; margin: 20px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.9rem; color: #a0a0a0;"><span style="color: #a855f7;">import</span> { QRCodefy } <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'qrcodefy'</span>;

<span style="color: #a855f7;">const</span> <span style="color: #f97316;">qr</span> = <span style="color: #a855f7;">new</span> <span style="color: #3b82f6;">QRCodefy</span>(<span style="color: #22c55e;">'https://example.com'</span>);

<span style="color: #666;">// Render in terminal</span>
<span style="color: #a855f7;">await</span> qr.<span style="color: #3b82f6;">toTerminal</span>();

<span style="color: #666;">// Save to file</span>
<span style="color: #a855f7;">await</span> qr.<span style="color: #3b82f6;">toFile</span>(<span style="color: #22c55e;">'./qrcode.png'</span>);

<span style="color: #666;">// Get as Data URL (for HTML &lt;img&gt;)</span>
<span style="color: #a855f7;">const</span> <span style="color: #f97316;">dataUrl</span> = <span style="color: #a855f7;">await</span> qr.<span style="color: #3b82f6;">toDataURL</span>();</code></pre>
  </div>

  <!-- Integrations Section -->
  <div id="integrations" style="padding: 40px 20px; border-bottom: 1px solid #333;">
    <h2 style="font-size: 2rem; margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">💡 Integrations</h2>
    <p style="color: #a0a0a0; margin-bottom: 30px;">Here's where QRCodefy shines. See how it integrates seamlessly with the most popular WhatsApp libraries.</p>

  <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 25px; margin: 25px 0;">
      <h3 style="color: #3b82f6; margin-top: 0; margin-bottom: 15px;">1️⃣ With @whiskeysockets/baileys</h3>
      <p style="color: #a0a0a0; margin-bottom: 20px;">Baileys emits a raw connection string. QRCodefy instantly transforms it into a scannable QR in your log.</p>
      <pre style="background: #111; border: 1px solid #333; border-radius: 8px; padding: 15px; overflow-x: auto; margin: 15px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.85rem; color: #a0a0a0;"><span style="color: #a855f7;">import</span> { makeWASocket, useMultiFileAuthState } <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'@whiskeysockets/baileys'</span>;
<span style="color: #a855f7;">import</span> { QRCodefy } <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'qrcodefy'</span>;

<span style="color: #a855f7;">async function</span> <span style="color: #3b82f6;">connectToWhatsApp</span>() {
  <span style="color: #a855f7;">const</span> { state, saveCreds } = <span style="color: #a855f7;">await</span> <span style="color: #3b82f6;">useMultiFileAuthState</span>(<span style="color: #22c55e;">'auth_info_baileys'</span>);
  <span style="color: #a855f7;">const</span> <span style="color: #f97316;">sock</span> = <span style="color: #3b82f6;">makeWASocket</span>({ auth: state });

  sock.ev.<span style="color: #3b82f6;">on</span>(<span style="color: #22c55e;">'connection.update'</span>, <span style="color: #a855f7;">async</span> (update) => {
    <span style="color: #a855f7;">const</span> { connection, lastDisconnect, qr } = update;

  <span style="color: #a855f7;">if</span> (qr) {
      <span style="color: #666;">// 🔥 THE MAGIC HAPPENS HERE</span>
      console.<span style="color: #3b82f6;">log</span>(<span style="color: #22c55e;">'Scan the QR Code below:'</span>);
      <span style="color: #a855f7;">const</span> <span style="color: #f97316;">qrcode</span> = <span style="color: #a855f7;">new</span> <span style="color: #3b82f6;">QRCodefy</span>(qr);
      <span style="color: #a855f7;">await</span> qrcode.<span style="color: #3b82f6;">toTerminal</span>(<span style="color: #a855f7;">true</span>);
    }
  });
}</code></pre>
    </div>

  <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 25px; margin: 25px 0;">
      <h3 style="color: #3b82f6; margin-top: 0; margin-bottom: 15px;">2️⃣ With EvolutionAPI (Webhooks)</h3>
      <p style="color: #a0a0a0; margin-bottom: 20px;">If you have a backend consuming EvolutionAPI, you often receive the QR Code Base64 via JSON. Use QRCodefy to save it as an image.</p>
      <pre style="background: #111; border: 1px solid #333; border-radius: 8px; padding: 15px; overflow-x: auto; margin: 15px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.85rem; color: #a0a0a0;"><span style="color: #a855f7;">import</span> express <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'express'</span>;
<span style="color: #a855f7;">import</span> { QRCodefy } <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'qrcodefy'</span>;

<span style="color: #a855f7;">const</span> <span style="color: #f97316;">app</span> = <span style="color: #3b82f6;">express</span>();
app.<span style="color: #3b82f6;">use</span>(express.<span style="color: #3b82f6;">json</span>());

app.<span style="color: #3b82f6;">post</span>(<span style="color: #22c55e;">'/webhook/evolution'</span>, <span style="color: #a855f7;">async</span> (req, res) => {
  <span style="color: #a855f7;">const</span> { event, data } = req.body;

  <span style="color: #a855f7;">if</span> (event === <span style="color: #22c55e;">'qrcode.updated'</span> && data.qrcode) {
  <span style="color: #a855f7;">const</span> <span style="color: #f97316;">qrManager</span> = <span style="color: #a855f7;">new</span> <span style="color: #3b82f6;">QRCodefy</span>(data.qrcode);
    
  <span style="color: #666;">// Show in server log</span>
  <span style="color: #a855f7;">await</span> qrManager.<span style="color: #3b82f6;">toTerminal</span>();

  <span style="color: #666;">// Save to public folder</span>
  <span style="color: #a855f7;">await</span> qrManager.<span style="color: #3b82f6;">toFile</span>(<span style="color: #22c55e;">'./public/qrcodes/session.png'</span>);
  }
  
  res.<span style="color: #3b82f6;">sendStatus</span>(<span style="color: #f97316;">200</span>);
});</code></pre>
    </div>

  <div style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 25px; margin: 25px 0;">
      <h3 style="color: #3b82f6; margin-top: 0; margin-bottom: 15px;">3️⃣ With WhatsApp-Web.js</h3>
      <pre style="background: #111; border: 1px solid #333; border-radius: 8px; padding: 15px; overflow-x: auto; margin: 15px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.85rem; color: #a0a0a0;"><span style="color: #a855f7;">import</span> { Client } <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'whatsapp-web.js'</span>;
<span style="color: #a855f7;">import</span> { QRCodefy } <span style="color: #a855f7;">from</span> <span style="color: #22c55e;">'qrcodefy'</span>;

<span style="color: #a855f7;">const</span> <span style="color: #f97316;">client</span> = <span style="color: #a855f7;">new</span> <span style="color: #3b82f6;">Client</span>();

client.<span style="color: #3b82f6;">on</span>(<span style="color: #22c55e;">'qr'</span>, <span style="color: #a855f7;">async</span> (qr) => {
  console.<span style="color: #3b82f6;">log</span>(<span style="color: #22c55e;">'📱 Scan this QR Code:'</span>);
  <span style="color: #a855f7;">const</span> <span style="color: #f97316;">qrcode</span> = <span style="color: #a855f7;">new</span> <span style="color: #3b82f6;">QRCodefy</span>(qr);
  <span style="color: #a855f7;">await</span> qrcode.<span style="color: #3b82f6;">toTerminal</span>();
  <span style="color: #a855f7;">await</span> qrcode.<span style="color: #3b82f6;">toFile</span>(<span style="color: #22c55e;">'./public/whatsapp-qr.png'</span>);
});

client.<span style="color: #3b82f6;">initialize</span>();</code></pre>
    </div>
  </div>

  <!-- API Reference Section -->
  <div id="api" style="padding: 40px 20px; border-bottom: 1px solid #333;">
    <h2 style="font-size: 2rem; margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">📚 API Reference</h2>

  <h3 style="font-size: 1.5rem; margin: 30px 0 15px; color: #3b82f6;">Constructor</h3>
    <h4 style="color: #a855f7; margin: 20px 0 10px; font-family: 'JetBrains Mono', monospace;">new QRCodefy(data: string, options?: QRCodeOptions)</h4>
    <p style="color: #a0a0a0; margin-bottom: 20px;">Instantiates the class with data (Text, URL, or Base64).</p>

  <table style="width: 100%; border-collapse: collapse; margin: 20px 0; font-size: 0.9rem;">
      <thead>
        <tr>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Parameter</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Type</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">data</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">string</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;">The content to encode (URL, text, or Base64)</td>
        </tr>
        <tr>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">options</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">object</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;">Optional configuration</td>
        </tr>
      </tbody>
    </table>

  <h3 style="font-size: 1.5rem; margin: 40px 0 15px; color: #3b82f6;">Methods</h3>

  <h4 style="color: #a855f7; margin: 25px 0 10px; font-family: 'JetBrains Mono', monospace;">toTerminal(small?: boolean): Promise&lt;void&gt;</h4>
    <p style="color: #a0a0a0; margin-bottom: 15px;">Renders the QR Code using ANSI/ASCII characters.</p>

  <table style="width: 100%; border-collapse: collapse; margin: 15px 0; font-size: 0.9rem;">
      <thead>
        <tr>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Parameter</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Type</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Default</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">small</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">boolean</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">true</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;">Use <code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">false</code> if QR Code is too dense/large</td>
        </tr>
      </tbody>
    </table>

  <h4 style="color: #a855f7; margin: 25px 0 10px; font-family: 'JetBrains Mono', monospace;">toFile(path: string): Promise&lt;void&gt;</h4>
    <p style="color: #a0a0a0; margin-bottom: 15px;">Saves the image to disk. Format is detected by extension.</p>

  <table style="width: 100%; border-collapse: collapse; margin: 15px 0; font-size: 0.9rem;">
      <thead>
        <tr>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Parameter</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Type</th>
          <th style="padding: 12px 15px; text-align: left; border-bottom: 1px solid #333; background: #1a1a1a; color: #f5f5f5;">Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">path</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;"><code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">string</code></td>
          <td style="padding: 12px 15px; border-bottom: 1px solid #333; color: #a0a0a0;">File path with extension (<code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">.png</code>, <code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">.svg</code>)</td>
        </tr>
      </tbody>
    </table>

  <h4 style="color: #a855f7; margin: 25px 0 10px; font-family: 'JetBrains Mono', monospace;">toDataURL(): Promise&lt;string&gt;</h4>
    <p style="color: #a0a0a0; margin-bottom: 20px;">Returns the string formatted as <code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">data:image/png;base64,...</code> ready to be placed in an HTML <code style="background: #1a1a1a; padding: 2px 6px; border-radius: 4px; color: #a855f7;">&lt;img src="..." /&gt;</code> tag.</p>
  </div>

  <!-- Configuration Options Section -->
  <div id="config" style="padding: 40px 20px;">
    <h2 style="font-size: 2rem; margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">🔧 Configuration Options</h2>
    <pre style="background: #1a1a1a; border: 1px solid #333; border-radius: 12px; padding: 20px; overflow-x: auto; margin: 20px 0;"><code style="font-family: 'JetBrains Mono', monospace; font-size: 0.9rem; color: #a0a0a0;"><span style="color: #a855f7;">const</span> <span style="color: #f97316;">qr</span> = <span style="color: #a855f7;">new</span> <span style="color: #3b82f6;">QRCodefy</span>(<span style="color: #22c55e;">'data'</span>, {
  errorCorrectionLevel: <span style="color: #22c55e;">'M'</span>, <span style="color: #666;">// L, M, Q, H</span>
  margin: <span style="color: #f97316;">4</span>,
  width: <span style="color: #f97316;">256</span>,
  color: {
    dark: <span style="color: #22c55e;">'#000000'</span>,
    light: <span style="color: #22c55e;">'#ffffff'</span>
  }
});</code></pre>
  </div>

  <!-- Footer -->
  <div style="text-align: center; padding: 40px 20px; border-top: 1px solid #333; margin-top: 20px;">
    <p style="color: #a0a0a0; margin-bottom: 15px;">Made with 💜 for the Bot Developer Community</p>
    <a href="https://github.com/purecore/qrcodefy" style="color: #a855f7; text-decoration: none; font-weight: 600; padding: 10px 20px; border: 1px solid #a855f7; border-radius: 25px; transition: all 0.2s;">⭐ Star us on GitHub</a>
  </div>
</div>