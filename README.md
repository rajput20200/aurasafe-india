# 🛡️ AuraSafe India 3.0

### Women's Safety & Emergency Assistance Web Application

AuraSafe India is a **mobile-first women's safety web application prototype** designed around fast emergency access, location awareness, discreet safety tools, commute monitoring, trusted contacts, and incident documentation.

The project combines **HTML, CSS, JavaScript, browser APIs, and Leaflet.js** to create an interactive safety-focused experience that works directly in the browser.

> 🚀 **Live Demo:** https://rajput20200.github.io/aurasafe-india/

---

## ✨ Key Features

### 🚨 Multi-Trigger SOS

AuraSafe provides multiple ways to activate its emergency flow:

* Long-press SOS activation
* Multi-tap activation
* Device-shake detection using the Device Motion API
* Voice-triggered emergency keywords
* 5-second cancellation countdown
* PIN-based cancellation

The SOS interaction logic is implemented directly in JavaScript using touch, mouse, motion, and speech events.

---

### 📍 Live Location Tracking

The Track section uses the browser's **Geolocation API** to continuously obtain the device position.

The application:

* Reads latitude and longitude
* Updates the displayed coordinates
* Updates the location marker
* Centers the interactive map around the current position
* Uses high-accuracy geolocation when available

---

### 🗺️ Interactive Safety Map

AuraSafe uses **Leaflet.js** to display an interactive map with a dynamic location marker.

The map uses Carto map tiles and updates the marker as the user's location changes.

---

### 🎙️ Voice Emergency Detection

The application uses browser speech recognition where supported.

It listens for predefined emergency phrases such as:

* `help me`
* `bachao`
* `emergency`
* `save me`

When a matching phrase is detected, the emergency flow can be triggered.

---

### 🕵️ Discreet Decoy Mode

AuraSafe includes a calculator-style decoy interface designed to provide a discreet alternative screen.

The calculator can also interact with the application's PIN logic and emergency flow.

---

### 📞 Emergency Assistance

The Shield section provides quick access to Indian emergency channels including:

* **112 — All-In-One Response**
* **1091 — Women Response Grid**

The interface uses device-supported telephone links for quick access.

---

### 🚌 Commute Safety Tools

The Commute section includes:

* Destination-based safety check-in
* Transit monitoring interface
* Vehicle/registration number logging
* Support for common Indian transport scenarios
* Simulated incoming-call decoy functionality

## The current implementation provides browser-side interaction and interface logic for these features.

### 🤖 Aura AI Safety Assistant

Aura AI provides an interactive safety guidance interface.

The current implementation is a **rule-based assistant**, using predefined responses and keyword matching rather than a connected external AI model.

This makes it a good demonstration of:

* Natural-language input handling
* Conditional logic
* Dynamic chat UI
* Safety-oriented response flows

---

### 👥 Trusted Safety Circle

Users can add trusted contacts by entering:

* Name
* Mobile number
* Relationship

The application maintains these contacts locally for use within the safety interface.

---

### 📝 Incident & Evidence Vault

The application records emergency incident information such as:

* Timestamp
* Location coordinates
* Emergency activation details

The incident information is stored locally in the browser and rendered inside the Evidence Vault.

---

### 🌐 Multilingual Interface

AuraSafe includes interface translations for:

* 🇬🇧 English
* 🇮🇳 Hindi
* Bengali
* Marathi
* Tamil
* Telugu
* Punjabi
* Gujarati
* Kannada
* Malayalam

The language selector and translation dictionary are built directly into the application.

---

### ♿ Accessibility Features

The interface includes accessibility-oriented display options:

* Large-text mode
* High-contrast mode
* Responsive mobile layout

The application uses CSS variables to dynamically adjust text scale, contrast, colors, and interface appearance.

---

### 🔋 Device & Network Diagnostics

AuraSafe can display browser/device information including:

* Battery level
* Network status
* Voice recognition availability
* Safety/risk context indicators

The application listens for online/offline changes and updates the interface accordingly.

---

# 📱 Application Structure

| Section        | Purpose                               |
| -------------- | ------------------------------------- |
| 🛡️ **Shield** | SOS and emergency assistance          |
| 📍 **Track**   | Location tracking and interactive map |
| 🚌 **Commute** | Travel safety and transit tools       |
| 🤖 **Aura AI** | Rule-based safety guidance            |
| 🔐 **Vault**   | Trusted contacts and incident records |

These five sections form the application's primary navigation structure.

---

# 🛠️ Technology Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* Responsive / mobile-first design
* CSS animations
* CSS variables
* DOM manipulation
* Event-driven JavaScript

### Browser APIs

* Geolocation API
* Device Motion API
* Web Speech API
* MediaDevices API
* Battery Status API
* LocalStorage API

### Libraries & Services

* Leaflet.js
* Carto map tiles
* Boxicons
* Google Maps links
* WhatsApp Web/API links

Leaflet and Boxicons are loaded as external frontend dependencies in the application.

---

# 🧠 What I Learned From This Project

Building AuraSafe India helped me explore:

* Designing mobile-first safety interfaces
* Handling multiple user interaction patterns
* Working with browser hardware APIs
* Implementing real-time geolocation updates
* Building interactive maps
* Managing client-side application state
* Creating multilingual interfaces
* Designing accessibility controls
* Working with browser permissions
* Creating responsive UI components
* Building interactive emergency workflows
* Structuring a larger single-page JavaScript application

---

# 🔐 Data & Security Approach

AuraSafe India is currently a **client-side web application prototype**.

Application settings, contacts, and incident records are stored locally using the browser's `localStorage`. For example, the user's configured PIN and trusted-contact information are written to local browser storage.

The current version does **not** have a cloud backend or production database.

Therefore, this project should be understood as a **frontend prototype demonstrating safety-focused interaction and browser technology**, rather than a production emergency-response platform.

---

# ⚠️ Prototype Disclaimer

AuraSafe India is an **educational and portfolio project**.

Some features simulate or demonstrate emergency workflows within the browser. The application does not provide direct integration with police, emergency-response centers, or a dedicated emergency dispatch backend.

For real emergencies, users should contact the appropriate official emergency services.

The legal-information section inside the prototype is also intended for demonstration and should not be treated as professional legal advice.

---

# 🚀 Future Development

The next version could introduce:

* 🔐 Secure backend authentication
* 🗄️ Cloud database integration
* 🔒 Proper encrypted data storage
* 👥 Secure real-time contact sharing
* 🔔 Push notifications
* 📡 Real-time location sharing
* ☁️ Secure cloud evidence storage
* 🤖 Integration with a real AI service
* 🚨 Emergency-service API integrations
* 🔑 Stronger authentication and authorization
* 🧪 Automated testing
* 🛡️ Production-grade security architecture

---

# 📂 Project Structure

Currently, AuraSafe India is implemented as a single-page web application:

```text
aurasafe-india/
│
├── index.html
└── README.md
```

The main application contains the HTML structure, CSS styling, and JavaScript functionality required to run the prototype.

---

# 🌐 Live Demo

### [Open AuraSafe India](https://rajput20200.github.io/aurasafe-india/)

Try the different sections:

**Shield → Track → Commute → Aura AI → Vault**

---

# 👩‍💻 Project Information

**Project:** AuraSafe India 3.0
**Category:** Women's Safety Web Application
**Type:** Frontend / Browser-Based Prototype
**Platform:** Web
**Deployment:** GitHub Pages

---

## ⭐ Portfolio Highlight

AuraSafe India demonstrates how **frontend development, browser APIs, interactive mapping, accessibility, localization, and user-centered safety workflows** can be combined into a single responsive web application.

Built as a portfolio project to explore practical JavaScript development and safety-focused product design.
