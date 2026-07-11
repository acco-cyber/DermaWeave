DermaWeave 🧥✨ (Medical-Grade Inclusive Fashion)
The first AI agent that blends Skin AI, Fabric Science, and Apparel Virtual Try-On to solve the real problem of sensitive skin and contact dermatitis in fashion.

🔗 Live Demo: https://derma-weave.vercel.app/🏆 Hackathon: YouCam API Skin AI & Apparel VTO Hackathon

🧠 The Problem
People with compromised skin barriers (eczema, psoriasis, acne, reactive skin) suffer from contact dermatitis caused by rough fabrics, synthetic blends, and heavy wool. Online shopping is a guessing game that often leads to skin flare-ups and high return rates.

💡 The Solution: DermaWeave
DermaWeave acts as an Agentic AI Shopping Assistant. It uses the YouCam Skin AI API to analyze a user's skin barrier, calculates a Skin Vulnerability Score (SVS), and automatically locks/padlocks clothing items in the storefront that would cause micro-tears and irritation. It then uses the YouCam Apparel VTO API to let them safely try on hypoallergenic alternatives.

⚙️ How It Works (The Agentic Workflow)
Biometric Scan: User captures/uploads a selfie.
Skin AI Analysis: The image is sent to the YouCam Skin AI API to extract Redness and Texture metrics.
The Logic Engine: We calculate a Skin Vulnerability Score (SVS) using the formula: Math.round((redness * 0.6) + (texture * 0.4)).
Storefront Filtration: If the SVS is high, the AI Agent automatically filters the catalog, padlocking high-friction items (like wool) and showcasing safe fabrics (like bamboo and silk).
Apparel VTO: Users click "Try On" to generate a Virtual Try-On of the safe clothing item using the YouCam Apparel VTO API.
🚀 Features
AI Skin Barrier Scan: Real-time biometric scanning UI with SVS calculation.
Treatment Plan: The AI Agent prescribes a dermatological treatment plan (ceramides, gentle cleansers) based on the scan.
Locked Storefront: Items dangerous for the user's skin are literally padlocked and grayed out.
Inspo AI Deconstructor: Upload a photo of an outfit you like; the AI analyzes the fabric weave, predicts its irritation risk, and finds a safe DermaWeave alternative.
Generative VTO Grid: Generates a 2x2 grid of safe colorway variations for the user to try on instantly.
Style Presets & Filter Canvas: One-click lifestyle presets ("Sleep & Recovery", "Formal & Office") and positive/negative filter toggles (+ Breathable, - Synthetics).
🛠 Tech Stack
Frontend: React.js (via CDN for zero-build deployment), Tailwind CSS, Framer Motion concepts, Lucide Icons.
Backend Logic: Node.js/Express ready (Fail-safe mechanism implemented to ensure 100% uptime during live demo).
APIs Used:
YouCam Skin AI API
YouCam Apparel VTO API
📷 Screenshots
(Add your screenshots here before submitting to Devpost)

🏃 Run Locally
Because this prototype uses React via CDN, it requires zero installation.

Clone the repo.
Open index.html in your browser.
That's it!
Scroll down and click "Commit changes..." again.
