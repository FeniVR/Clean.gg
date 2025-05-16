
# Clean.gg

**Clean.gg** is multiplayer and VR moderation & security system for game developers.  
It offers a powerful Trust Score system, toxicity detection (inspired by GGWP), Discord integration, web panel, REST API, and a Unity SDK.

---

## Features

- **Unity SDK** – Easy integration with your Unity-based game
- **Trust Score System** – Dynamic reputation system based on behavior
- **Toxicity Detection** – Automatic analysis and handling of toxic behavior
- **Web Panel** – Manage players, reports, bans, and roles
- **Discord Webhooks** – Get real-time alerts for bans, reports, and actions
- **REST API** – Full control over Clean.gg from your backend
- **Roles & Permissions** – For moderators, admins, and developers

---

## Tech Stack

- **Frontend**: Next.js + TailwindCSS + ShadCN UI
- **Backend**: FastAPI (Python) + PostgreSQL + Redis
- **SDK**: C# for Unity
- **Auth**: Discord OAuth2 + JWT
- **Hosting**: Vercel / Railway / Docker (production ready)

---

## Installation

### Web Panel & API (dev)

# Clone
git clone https://github.com/fenivr/clean.gg.git
cd clean.gg

# Backend setup
cd clean-api
pip install -r requirements.txt
uvicorn main:app --reload

# Frontend setup
cd ../clean-panel-web
npm install
npm run dev

Unity SDK

Coming soon – located in /clean-sdk-unity


---

Contributing

We welcome PRs and issues!
Want to improve Clean.gg or add a feature? Fork this repo, submit your PR and let's build a safer multiplayer future together.


---

License

MIT License
© 2025 Night Labs Inc. / fenivr


---

Links

Discord: dc.gg/killyourself

Website: Coming soon

Contact: @fenivr - on discord
