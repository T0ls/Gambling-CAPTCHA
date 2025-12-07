# Scratch & Verify: The Gambling CAPTCHA

![Project Status](https://img.shields.io/badge/Status-PoC-orange) ![License](https://img.shields.io/badge/License-CC_BY_4.0-blue) ![Addiction-Level](https://img.shields.io/badge/Dopamine-High-red)

**Scratch & Verify** is a lightweight, zero-dependency JavaScript CAPTCHA that replaces the frustration of identifying traffic lights with the thrill of a scratch-off lottery ticket. It secures your website by exploiting the one vulnerability bots don't have: **a gambling addiction**.

## 📖 The Philosophy: The "Scratch & Verify" Protocol

*Why Gambling is the Ultimate Turing Test*

Forget image recognition and text distortion. The future of cybersecurity resides in **behavioral psychology**.

### 1. The Engagement Barrier
Traditional CAPTCHAs are an obstacle; this CAPTCHA is an opportunity.
* **Dopamine vs. Cortisol:** Instead of increasing user stress, we offer a hit of anticipatory dopamine.
* **Biometric Chaos:** The act of digitally "scratching" generates chaotic mouse/touch paths that are incredibly difficult for bots to replicate naturally.

### 2. The True "Humanity Check"
The system doesn't just check *if* you scratched the ticket, but *how* you react to the result.

**The Loop:**
1.  The user scratches the ticket.
2.  **The user wins.** (The system allows for a configurable win rate).
3.  A "Claim Prize" button appears alongside a "New Ticket" button.

**The Verification Logic:**
* **The Bot:** Detects the task is solved. Clicks "Claim Prize" immediately to proceed. Efficiency: 100%.
* **The Human:** Sees they won. The reptilian brain lights up. *If I won once, I can win again.* They ignore the destination URL. They click **"New Ticket"**. They win again. They click **"New Ticket"** again.

The system essentially certifies the user as a "Certified Human" the exact moment they **stop wanting to enter the site** because they are too busy scratching virtual pixels.

---

## 🚀 Features

* **Realistic Scratch Effect:** HTML5 Canvas-based scratch surface with "silver foil" gradients and particle debris.
* **SVG Ticket Generation:** Crisp, scalable vector graphics for the ticket background and text.
* **Win/Loss Logic:** Configurable logic for matching numbers (default: match 3 symbols to win).
* **Dopamine Reinforcement:** Includes a fireworks particle system upon winning.
* **Responsive Design:** Works on desktop (mouse) and mobile (touch).
* **Zero Dependencies:** Pure Vanilla JS and CSS.

## 📦 Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/gambling-captcha.git](https://github.com/your-username/gambling-captcha.git)
    ```

2.  **Run the demo:**
    Simply open the `index.html` file in any modern web browser. No build step or server is required.

    ```bash
    # Or serve it locally
    npx serve .
    ```

## ⚙️ Configuration

You can tweak the game mechanics by modifying the constants at the top of the `<script>` section in `index.html`:

```javascript
// How many winning numbers to generate (default: 3)
const WIN_COUNT = 3;

// Total cells on the ticket (default: 12)
const CELL_COUNT = 12;

// Percentage of the surface that must be scratched to auto-reveal (0.0 - 1.0)
let AUTO_SCRATCH_THRESHOLD = 0.80;

// How many matches are required to trigger a "Win" state
let MATCHES_TO_WIN = 3;

// The destination URL when the user finally decides to "Claim Prize"
const REDIRECT_URL = '[https://www.youtube.com/watch?v=IPFiKEm-oNI](https://www.youtube.com/watch?v=IPFiKEm-oNI)';
```
