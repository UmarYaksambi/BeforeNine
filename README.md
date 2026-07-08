# BeforeNine 🌅

> **A collaborative, offline-capable habit tracker to help you conquer your mornings.**  
> BeforeNine is a Progressive Web App (PWA) designed to build better routines through individual streak tracking, real-time team accountability, and comprehensive habit analytics.[cite: 2]

---
## 📸 Screenshots

<div align="center">
  <img src="https://github.com/UmarYaksambi/Assets/blob/main/BeforeNine/photo1.jpeg?raw=true" alt="BeforeNine Dashboard" width="45%" />
  <img src="https://github.com/UmarYaksambi/Assets/blob/main/BeforeNine/photo2.jpeg?raw=true" alt="Squad Sync Feature" width="45%" />
  <br>
  <img src="https://github.com/UmarYaksambi/Assets/blob/main/BeforeNine/photo3.jpeg?raw=true" alt="Mobile View" width="45%" />
</div>

---

## 🌍 Why This Project?

Building habits in isolation can be tough, and relying on apps that demand a constant internet connection creates friction. 

BeforeNine eliminates these barriers by providing:

- 📶 **Offline-first functionality as an installable PWA**[cite: 2]
- 🌐 **Seamless state synchronization with Supabase**[cite: 2]
- 🧠 **Individual streak and analytics calculation**[cite: 2]
- 🏫 **Social accountability through "Squad Sync"**[cite: 2]

Whether you are tracking your personal reading goals or making sure your startup team hits the gym, BeforeNine adapts to your workflow.

---

## ✨ Core Features

### 🧠 Advanced Habit Tracking

At its core, BeforeNine visually maps your consistency.

- **The Habit Grid**  
  A visual heatmap (`HabitGrid.jsx`) for tracking daily progress at a glance.[cite: 2]
- **Smart Streaks & Stats**  
  Domain logic (`streaks.js`, `stats.js`) automatically calculates current streaks, longest streaks, and completion percentages.[cite: 2]

### 🤝 Squad Sync

Habit tracking built for multiplayer.

- **Team Accountability**  
  The `SquadSync.jsx` module allows users to connect with friends and monitor collective progress.[cite: 2]
- **Quick Squad Stats**  
  View top performers and overall group consistency directly from the dashboard (`SquadQuickStats.jsx`).[cite: 2]

### 📶 Offline-First PWA Architecture

Built to feel like a native app on any device.

- **Installable**  
  Fully configured `manifest.webmanifest` and service workers allow you to add it directly to your home screen.[cite: 2]
- **Workbox Caching**  
  Utilizes Workbox (`workbox-1d305bb8.js`) to cache assets and handle offline habit logging seamlessly.[cite: 2]
- **Mobile Optimized**  
  Features dedicated mobile UI elements like `HabitCardMobile.jsx` for perfect responsiveness.[cite: 2]

---

## 🛠️ Technical Architecture

BeforeNine uses a modern, lightning-fast frontend stack.

| Layer               | Technology                 | Purpose                |
| ------------------- | -------------------------- | ---------------------- |
| **Framework**       | **React + Vite**           | UI & Build Tooling[cite: 2] |
| **Styling**         | **Tailwind CSS**           | Utility-first design[cite: 2] |
| **State Mgt**       | **Zustand**                | Global habit store (`useHabitStore.js`)[cite: 2] |
| **Database & Auth** | **Supabase (PostgreSQL)**  | Backend syncing & auth (`supabase.js`)[cite: 2] |
| **Offline/PWA**     | **Service Workers/Workbox**| Asset caching & offline mode[cite: 2] |

---

## 🚀 Getting Started

### Prerequisites

- Node.js **18+**
- npm / yarn
- Supabase Project (for database and auth)

### Installation

1. **Clone the repository**

```bash
git clone [https://github.com/UmarYaksambi/BeforeNine.git](https://github.com/UmarYaksambi/BeforeNine.git)
cd BeforeNine

```

2. **Install dependencies**


```bash
npm install

```

3. **Environment Configuration**


Create a `.env` file in the root directory and add your Supabase keys:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_anon_key
```

4. **Run the development server**


```bash
npm run dev
```

5. **Open in your browser**

```
http://localhost:5173
```

---

## 📂 Project Structure

```bash
BeforeNine/
├── public/                 # Static PWA icons[cite: 2]
├── src/                    # Source code[cite: 2]
│   ├── components/         # React UI Components (Grid, Cards, SquadSync)[cite: 2]
│   ├── db/                 # Supabase clients and table logic[cite: 2]
│   ├── domain/             # Core business logic (streaks, stats)[cite: 2]
│   ├── hooks/              # Custom React hooks (useAuth, useHabits)[cite: 2]
│   ├── store/              # Zustand global state (useHabitStore)[cite: 2]
│   └── utils/              # Helper functions (date formatting)[cite: 2]
├── index.html              # App entry point[cite: 2]
├── tailwind.config.js      # Tailwind styling configuration[cite: 2]
└── vite.config.js          # Vite build settings[cite: 2]

```

---

## 🤝 Contributing

Contributions are always welcome!

### How to contribute

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

Licensed under the **MIT License**.
See `LICENSE` for details.

---

<div align="center">
  <strong>Built with ❤️ to make building lasting habits simple, social, and accessible.</strong>
  <br><br>
  <a href="https://github.com/UmarYaksambi/BeforeNine">GitHub</a>
  &bull;
  <a href="https://beforenine.vercel.app">Live Website</a>
  &bull;
  <a href="https://buymeacoffee.com/UmarYaksambi">Buy Me a Coffee</a>
</div>

