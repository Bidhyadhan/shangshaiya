# shangshaiya
Global Heritage Silk and Original market place
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SHANGSHAIYA | Global Heritage Enterprise</title>
    <script src="https://unpkg.com/html5-qrcode"></script>
    <style>
        :root { --primary: #722f37; --accent: #daa520; --bg: #fffcf5; --safe: #27ae60; --alert: #c0392b; --ship: #3498db; --ai: #8e44ad; }
        body { font-family: 'Georgia', serif; margin: 0; background: var(--bg); color: #333; overflow-x: hidden; }
        
        /* 1. NAVIGATION & LANGUAGE */
        .top-bar { background: #1a1a1a; color: white; padding: 10px; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 1000; }
        .lang-btn { cursor: pointer; font-size: 0.75rem; margin-right: 10px; border: 1px solid #444; padding: 3px 8px; border-radius: 3px; }
        .lang-btn.active { background: var(--accent); color: black; border-color: var(--accent); }

        /* 2. HEADER & BRANDING */
        header { background: var(--primary); color: white; padding: 40px 20px; text-align: center; border-bottom: 5px solid var(--accent); }
        .hero-sub { font-style: italic; opacity: 0.9; margin-top: 5px; }

        .container { max-width: 1200px; margin: auto; padding: 20px; }

        /* 3. AGENT LEADERBOARD */
        .panel { background: white; border: 1px solid #ddd; padding: 20px; border-radius: 12px; margin-bottom: 25px; box-shadow: 0 4px 10px rgba(0,0,0,0.05); }
        .leader-row { display: flex; justify-content: space-between; padding: 8px 0; border-bottom: 1px solid #eee; }

        /* 4. PRODUCT CARDS & INDIGENOUS SPECS */
        .product-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        .card { background: white; border: 1px solid #ddd; padding: 20px; border-radius: 15px; position: relative; }
        .badge { position: absolute; top: 15px; right: 15px; font-size: 0.65rem; padding: 4px 10px; border-radius: 20px; color: white; font-weight: bold; }
        .indigenous-box { background: #fdf6e3; border: 1px dashed var(--accent); padding: 10px; margin-top: 15px; font-size: 0.8rem; border-radius: 8px; }
        
        /* 5. BUTTONS */
        .btn { padding: 12px; border: none; border-radius: 8px; font-weight: bold; cursor: pointer; width: 100%; margin-top: 10px; transition: 0.2s; }
        .btn-wa { background: #25D366; color: white; }
        .btn-scan { background: var(--accent); color: black; font-size: 1rem; }
        .btn-ai { background: var(--ai); color: white; }

        /* 6. ADMIN & SCANNER */
        #reader { width: 100%; max-width: 450px; margin: 15px auto; border: 4px solid var(--accent); display: none; }
        .admin-only { display: none; border-top: 5px solid var(--primary); padding-top: 30px; }
        .secure-dot { position: fixed; bottom: 5px; right: 5px; width: 10px; height: 10px; opacity: 0.05; cursor: pointer; }
    </style>
</head>
<body>

<div class="top-bar">
    <div>
        <span class="lang-btn active">English</span>
        <span class="lang-btn" onclick="alert('Dimasa UI Loading...')">Dimasa</span>
        <span class="lang-btn" onclick="alert('Assamese UI Loading...')">Assamese</span>
    </div>
    <div style="font-size: 0.7rem; letter-spacing: 1px;">HAFLONG | 2026</div>
</div>

<header>
    <h1>SHANGSHAIYA</h1>
    <p class="hero-sub">Indigenous Silk • Organic Hill Produce • Legal Heritage Export</p>
</header>

<div class="container">
    
    <div class="panel">
        <h3 style="margin-top:0;">🏆 Top Performers (Monthly)</h3>
        <div id="leader-list">
            <div class="leader-row"><span>#1 Agent Raktim</span><strong>₹18,500</strong></div>
            <div class="leader-row"><span>#2 Agent Priya</span><strong>₹12,200</strong></div>
        </div>
    </div>

    <div style="text-align:center; margin-bottom:40px;">
        <button class="btn btn-scan" onclick="startScanner()">📸 SCAN PRODUCT QR (AGENT ONLY)</button>
        <div id="reader"></div>
        <div id="scan-result" style="margin-top:15px; font-weight:bold;"></div>
    </div>

    <div class="product-grid" id="main-store"></div>

    <div id="admin-panel" class="admin-only">
        <h2 style="color:var(--primary); text-align:center;">MASTER CONTROL CENTER (BIDHYADHAN)</h2>
        
        <div class="panel" style="background: #f0f4f8;">
            <h3>📦 Inventory & Legal Editor</h3>
            <table style="width:100%; border-collapse: collapse;">
                <tr style="background:#eee;"><th>ID</th><th>Price</th><th>FSSAI</th><th>Dye Type</th></tr>
                <tr><td>RIGU01</td><td>2500</td><td>N/A</td><td>Natural Indigo</td></tr>
            </table>
        </div>

        <div class="panel" style="background: #fdf2ff; border: 2px solid var(--ai);">
            <h3 style="color:var(--ai);">🤖 Gemini AI Business Strategy</h3>
            <textarea id="ai-query" placeholder="Ask Gemini: How to export King Chilli to USA?" style="width:100%; height:80px;"></textarea>
            <button class="btn btn-ai" onclick="consultAI()">CONSULT GEMINI AI</button>
            <div id="ai-resp" style="margin-top:10px; font-style:italic; padding:10px; background:white; display:none;"></div>
        </div>

        <div class="panel">
            <h3>🚚 Live Transportation Rates</h3>
            <p>Current Petrol/Diesel Surcharge: <strong>12%</strong></p>
            <button onclick="alert('Rates Updated Globally')" style="padding:10px;">Sync All Delivery Charges</button>
        </div>
    </div>
</div>

<footer>
    <div style="text-align:center; padding:40px; background:#eee; font-size:0.75rem;">
        <p><strong>FSSAI:</strong> Verified | <strong>IT ACT 2000:</strong> Compliant | <strong>Dyeing:</strong> 100% Indigenous</p>
        <p>© 2026 SHANGSHAIYA ENTERPRISE. PROUDLY BORN IN HAFLONG.</p>
    </div>
</footer>

<div class="secure-dot" onclick="login()">.</div>

<script>
    const ADMIN_KEY = "123456";
    const CONTACT = "9401941416";

    // MASTER DATABASE
    let database = [
        {id: "ERI01", name: "Indigenous Eri Silk", price: 3500, type: "Textile", dye: "Indigo/Bark", fssai: false, legal: "🟢 Global Export Ready"},
        {id: "CHILLI09", name: "Haflong King Chilli", price: 200, type: "Food", dye: "N/A", fssai: true, legal: "🟡 Restricted (Check Permits)"},
        {id: "BAMBOO03", name: "Ash-Treated Basket", price: 550, type: "Craft", dye: "Wood Ash", fssai: false, legal: "🟢 Global Export Ready"}
    ];

    function render() {
        const store = document.getElementById('main-store');
        store.innerHTML = database.map(item => `
            <div class="card">
                <span class="badge" style="background:${item.fssai ? 'var(--safe)' : 'var(--primary)'}">
                    ${item.fssai ? 'FSSAI CERTIFIED' : item.type}
                </span>
                <h3>${item.name}</h3>
                <p style="font-size:1.4rem; font-weight:bold; color:var(--primary); margin:5px 0;">₹${item.price}</p>
                <div class="indigenous-box">
                    <strong>Indigenous Details:</strong><br>
                    🧵 Silk Type: ${item.type === 'Textile' ? 'Eri (Ahimsa)' : 'N/A'}<br>
                    🎨 Dyeing: ${item.dye}<br>
                    ⚖️ Legal: ${item.legal}
                </div>
                <button class="btn btn-wa" onclick="order('${item.name}')">ORDER VIA WHATSAPP</button>
            </div>
        `).join('');
    }

    function order(name) {
        window.open(`https://wa.me/${CONTACT}?text=Order+Request:+${name}`, '_blank');
    }

    function startScanner() {
        const reader = document.getElementById('reader');
        reader.style.display = 'block';
        const scanner = new Html5Qrcode("reader");
        scanner.start({ facingMode: "environment" }, { fps: 10, qrbox: 250 }, (text) => {
            const found = database.find(p => text.includes(p.id));
            if(found) {
                document.getElementById('scan-result').innerHTML = `
                    <div style="color:var(--safe)">✅ FOUND: ${found.name}<br>LEGAL STATUS: ${found.legal}</div>
                `;
                setTimeout(() => { order(`Agent Sale: ${found.name}`); }, 2000);
            }
            scanner.stop();
            reader.style.display = 'none';
        });
    }

    function consultAI() {
        const query = document.getElementById('ai-query').value;
        const resp = document.getElementById('ai-resp');
        resp.style.display = "block";
        resp.innerText = "Gemini AI is analyzing market trends for " + query + "...";
        setTimeout(() => {
            resp.innerHTML = "<strong>Gemini Advice:</strong> For Indigenous silk dyed with bark, target the 'Eco-Conscious' market in Germany. Ensure the Wood-Ash treatment is mentioned in the export story for 30% higher margins.";
        }, 1500);
    }

    function login() {
        if(prompt("Enter Admin Master Key:") === ADMIN_KEY) {
            document.getElementById('admin-panel').style.display = 'block';
            window.scrollTo(0, document.body.scrollHeight);
        }
    }

    render();
</script>
</body>
</html>
