# App Manager

Your complete mission control for building, tracking, and scaling apps in the web3 ecosystem. Built onchain with real-time collaboration powered by SpacetimeDB.

![Version](https://img.shields.io/badge/version-1.0.0-purple)
![License](https://img.shields.io/badge/license-MIT-blue)
![Built on Base](https://img.shields.io/badge/built%20on-Base-0052FF)

---

## 🌟 Overview

App Manager is a comprehensive dashboard that provides a unified view of all your applications with real-time synchronization, team collaboration, and AI-powered insights. Perfect for solo builders and growing teams shipping onchain.

---

## ✨ Features

### Core Features
- **📊 Real-time Dashboard**: Track all your apps with live updates via SpacetimeDB
- **✅ Task Management**: Full CRUD operations for tasks with priority levels
- **🏷️ Smart Tags**: Organize and categorize apps efficiently
- **🔗 Link Hub**: Centralized resource management
- **💬 Team Chat**: Real-time messaging with global/app-specific rooms and DMs
- **👤 User Profiles**: Public portfolio mode with shareable links

### Tier 1 Features
- **📈 Analytics Dashboard**: Visual metrics and performance tracking
- **🚀 Launch Templates**: Quick-start templates for new apps
- **🎨 Link Hub**: Organize all your important resources
- **🏷️ Smart Tags System**: Advanced categorization

### Tier A Features
- **🌐 Public Profile Mode**: Shareable portfolio of your apps
- **🔔 Smart Notifications**: Real-time alerts for tasks and updates
- **📊 Marketing Metrics**: Track downloads, revenue, users, engagement
- **⚙️ Custom Settings**: Personalize your experience

### Tier 2 Features
- **📝 Activity Timeline**: Complete audit log of all changes
- **📦 Version History**: Track releases with changelogs
- **⏱️ Time Tracker**: Log work hours per app/task
- **💾 Export Tools**: Full data backup capabilities

### Tier 3 Features (Advanced)
- **🧠 AI Insights**: Predictive analytics and health scores
- **🔌 Integrations Hub**: Connect GitHub, app stores, social media
- **🔗 Chainboard Sync**: Integration with [chainboard.elpeef.com](https://chainboard.elpeef.com) for team management and Jitsi meetings
- **📡 Real-time Collaboration**: Live sync across all team members

---

## 🛠️ Technology Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Database**: SpacetimeDB (Real-time sync)
- **Styling**: Tailwind CSS
- **UI Components**: shadcn/ui
- **Charts**: Recharts
- **Icons**: Lucide React
- **Blockchain**: Built for Base Chain

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn
- SpacetimeDB CLI (for local development)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd app-manager
```

2. Install dependencies:
```bash
npm install
```

3. Set up SpacetimeDB:
```bash
# Install SpacetimeDB CLI if you haven't
curl --proto '=https' --tlsv1.2 -sSf https://install.spacetimedb.com | sh

# Start local SpacetimeDB instance
spacetime start

# Publish the database module
cd spacetime-server
spacetime publish app-manager
```

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📁 Project Structure

```
├── src/
│   ├── app/              # Next.js app router
│   ├── components/       # React components
│   │   ├── ui/          # shadcn/ui components
│   │   ├── About.tsx    # About page
│   │   ├── Chat.tsx     # Chat system
│   │   └── ...          # Other feature components
│   ├── hooks/           # Custom React hooks
│   └── spacetime_module_bindings/  # Auto-generated SpacetimeDB types
├── spacetime-server/    # SpacetimeDB Rust module
│   └── src/
│       └── lib.rs       # Database schema & reducers
└── public/              # Static assets
```

---

## 🗄️ Database Schema

The app uses SpacetimeDB with the following main tables:

- **apps**: Core application data
- **tasks**: Task management with priorities
- **tags**: Categorization system
- **links**: Resource management
- **messages**: Chat system
- **notifications**: Alert system
- **profiles**: User settings
- **metrics**: Marketing analytics
- **activities**: Audit logs
- **versions**: Release tracking
- **time_entries**: Work hour logging
- **integrations**: External service connections

---

## 🎨 Features in Detail

### Real-time Chat
- Global chat room for all users
- App-specific chat rooms
- Direct messaging between users
- Emoji reactions
- Online status indicators
- Message history

### AI Insights
- App health scores
- Development time forecasts
- Priority task alerts
- Performance predictions
- Pattern recognition

### Integrations Hub
- GitHub repository tracking
- App Store Connect stats
- Social media post scheduling
- Custom API integrations
- Sync status monitoring

### Chainboard Integration
- Sync apps and tasks to [chainboard.elpeef.com](https://chainboard.elpeef.com)
- Jitsi video meetings
- Team collaboration tools
- Cross-platform compatibility

---

## 🔧 Configuration

The app automatically configures SpacetimeDB connection. For custom settings, modify:

```typescript
// src/hooks/useSpacetimeDB.ts
const MODULE_NAME = 'app-manager';
const HOST = 'wss://testnet.spacetimedb.com';
```

---

## 📱 Mobile Support

- Fully responsive design
- Collapsible sidebar for mobile
- Touch-optimized controls
- Adaptive layouts

---

## 🤝 Contributing

Contributions are welcome! This is an open-source project built for the community.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the MIT License.

---

## 🙏 Credits

- Built by web3 builders for web3 builders
- Powered by [SpacetimeDB](https://spacetimedb.com) for real-time collaboration
- UI components from [shadcn/ui](https://ui.shadcn.com)
- Built for [Base Chain](https://base.org)

---

## 🔗 Links

- **Website**: [rantai.elpeef.com](https://rantai.elpeef.com)
- **GitHub**: [mrbrightsides](https://github.com/mrbrightsides)
- **Chainboard**: [chainboard.elpeef.com](https://chainboard.elpeef.com)

## 📧 Contact

For questions, feedback, or collaboration opportunities, reach out through the links above.

---

Built with 💜 for the onchain ecosystem. Ship fast, ship onchain! 🚀
