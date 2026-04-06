# 🌟 Illuminate Hope — End-to-End Business Registration Solution

> Empowering South African entrepreneurs with a seamless, automated path from idea to operating business.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Solution Architecture](#solution-architecture)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

**Illuminate Hope** is an end-to-end business registration and onboarding solution built for South African entrepreneurs. It automates the critical steps required to legally establish and digitally launch a business — removing friction, reducing cost, and cutting down weeks of admin to a streamlined process.

Whether you're a first-time founder or helping others formalise their businesses, this solution walks you through every step — from legal registration to having a live online presence.

---

## Features

| Module | Description | Status |
|--------|-------------|--------|
| 🏛️ **CIPC Registration** | Company registration with the Companies and Intellectual Property Commission | ✅ Complete |
| 📄 **Annual Returns (AR)** | Automated Annual Return filing and reminders | ✅ Complete |
| 👤 **Beneficial Ownership (BO)** | Beneficial Ownership register submission | ✅ Complete |
| 🌐 **Domain Registration** | Business domain name search and registration | ✅ Complete |
| 📧 **Email Setup** | Professional business email address provisioning | ✅ Complete |
| 🖥️ **Website** | Business website creation and hosting | ✅ Complete |

---

## Solution Architecture

```
illuminate-hope/
│
├── registration/
│   ├── cipc/          # CIPC company registration workflow
│   ├── annual-returns/ # AR filing automation
│   └── beneficial-ownership/ # BO register submission
│
├── digital/
│   ├── domain/        # Domain registration and DNS setup
│   ├── email/         # Business email provisioning
│   └── website/       # Website setup and hosting
│
├── client/
│   └── dashboard/     # Client status tracking portal
│
└── docs/              # Documentation and guides
```

---

## Getting Started

### Prerequisites

- Node.js v18+ or Python 3.10+
- Git
- A CIPC account (for registration workflows)
- Domain registrar API credentials (e.g., Afrihost, Domains.co.za)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/illuminate-hope.git

# Navigate into the project
cd illuminate-hope

# Install dependencies
npm install   # or pip install -r requirements.txt

# Copy environment variables
cp .env.example .env
```

### Configuration

Edit `.env` with your credentials:

```env
CIPC_USERNAME=your_cipc_username
CIPC_PASSWORD=your_cipc_password
DOMAIN_API_KEY=your_registrar_api_key
EMAIL_PROVIDER_KEY=your_email_api_key
```

> ⚠️ **Never commit your `.env` file.** It is already listed in `.gitignore`.

---

## Usage

### Run the full onboarding pipeline

```bash
npm run start
# or
python main.py
```

### Run individual modules

```bash
# CIPC Registration only
npm run register:cipc

# Domain + Email setup only
npm run setup:digital
```

---

## Roadmap

- [ ] SARS eFiling tax registration integration
- [ ] B-BBEE affidavit auto-generation for EMEs
- [ ] Annual return renewal reminders (email/SMS)
- [ ] Bank account opening referral partnerships
- [ ] Self-service client web portal
- [ ] Multi-client / agency mode

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "feat: add your feature"`
4. Push to your branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for code standards and guidelines.

---

## Built With

- **Python / Node.js** — Backend automation
- **React** — Client dashboard frontend
- **GitHub Actions** — CI/CD pipeline
- **Supabase** — Database and auth

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Illuminate Hope**
- GitHub: [@your-username](https://github.com/your-username)
- Email: info@illuminatehope.co.za
- Website: [www.illuminatehope.co.za](https://www.illuminatehope.co.za)

---

> *"Illuminating the path for every South African entrepreneur."* 🇿🇦
