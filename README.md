🧥 DermaWeave
Medical-Grade Inclusive Fashion
Live DemoHackathonFrameworkStyling

DermaWeave is an Agentic AI shopping assistant that bridges the gap between dermatology and e-commerce. By combining YouCam's Skin AI and Apparel VTO APIs, it creates a hyper-personalized storefront that protects compromised skin barriers.

📑 Table of Contents
🎯 The Problem
💡 The Solution
⚙️ Architecture & Agentic Workflow
✨ Key Features
🔌 YouCam API Integration
🛠 Tech Stack
🚀 Local Setup
🎯 The Problem
People with compromised skin barriers (eczema, psoriasis, acne, reactive skin) suffer from contact dermatitis caused by rough fabrics, synthetic blends, and heavy wool. Currently, online shopping is a guessing game that often leads to skin flare-ups, discomfort, and high return rates for retailers.

💡 The Solution
DermaWeave acts as an Intelligent AI Stylist and Dermatologist. Instead of treating skin analysis and fashion as separate features, DermaWeave unifies them. The AI scans the user's skin, calculates a Skin Vulnerability Score (SVS), and automatically "padlocks" clothing items in the storefront that would cause micro-tears and irritation. It then prescribes a treatment plan and allows the user to virtually try on guaranteed-safe fabrics.

⚙️ Architecture & Agentic Workflow
DermaWeave isn't just a wrapper—it's an agentic workflow where the output of the Skin AI directly manipulates the UI and available inventory of the Apparel VTO storefront.

Biometric Capture: The user takes a selfie via webcam or upload.
Skin AI Analysis: The image is sent to the YouCam Skin AI API to extract Redness and Texture metrics.
The Logic Engine: The backend calculates a Skin Vulnerability Score (SVS) using the formula: Math.round((redness * 0.6) + (texture * 0.4)).
Storefront Filtration: If the SVS is > 50 (Highly Reactive), the AI Agent automatically filters the catalog. High-friction items (like Lambswool or Polyester) are rendered with a CSS grayscale filter, padlocked, and their "Add to Cart" / "Try On" events are disabled.
Apparel VTO: When the user clicks a "Safe" item, the original selfie and the clothing's vto_model_id are sent to the YouCam Apparel VTO API, generating a 2x2 grid of colorway variations for the user to choose from.
✨ Key Features
🔬 AI Skin Barrier Scan: Real-time biometric scanning UI with SVS calculation.
🧴 Prescribed Treatment Plan: The AI Agent reads the scan results and prescribes a holistic dermatological treatment plan (e.g., ceramides, hypochlorous acid) to heal the barrier.
🔒 Locked Storefront: Items dangerous for the user's skin are literally padlocked, grayed out, and unclickable, ensuring 100% safety.
🧩 Inspo AI Deconstructor: Users can upload a photo of an outfit they love. The AI analyzes the fabric weave, predicts its irritation risk, and finds a safe DermaWeave alternative.
📸 Generative VTO Grid: Generates a 2x2 grid of safe colorway variations simultaneously using the Apparel VTO API, giving users immediate choice.
🎚️ Style Presets & Filter Canvas: One-click lifestyle presets ("Sleep & Recovery", "Formal & Office") and positive/negative filter toggles (+ Breathable, - Synthetics).
🔌 YouCam API Integration
This project utilizes the Skin AI + Apparel VTO combined track.

Skin AI API:
Endpoint: POST /api/analyze-skin
Usage: Forwards the user's image to YouCam to retrieve redness and texture scores. These numbers drive the entire UI logic.
Apparel VTO API:
Endpoint: POST /api/vto
Usage: Takes the user's original selfie and the vto_model_id of a safe clothing item, returning a generative image of the user wearing the item.
🛠 Tech Stack
Frontend: React 18 (via Babel Standalone for zero-build deployment), Tailwind CSS (CDN).
Backend Logic: Node.js/Express ready (with Multer for image handling). Note: This live demo uses a mocked frontend agent to simulate the backend API responses for 100% uptime during judging.
APIs: YouCam Skin AI, YouCam Apparel VTO.
🚀 Local Setup
Because this prototype is built with React via CDN, it requires zero installation and no build steps.

Clone the repository:
git clone https://github.com/acco-cyber/DermaWeave.git
Navigate to the folder:
bash

cd DermaWeave
Open index.html in your preferred browser.
That's it! The app is fully functional.
<div align="center">

Built for the YouCam API Hackathon 🏆
Showcasing the future of inclusive, medical-grade consumer fashion.

</div>
```


