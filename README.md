# CommitMind 🧠
### The AI That Never Lets Important Commitments Slip

**CommitMind** is an AI-powered commitment intelligence platform designed to turn scattered promises into clear, actionable responsibilities.

## 🚨 The Problem

Important commitments are buried in emails, documents, and meeting notes. People forget follow-ups, miss deadlines, and struggle to track who is responsible for what.

Traditional task managers often require users to manually create tasks after a commitment has already been made.

## 💡 Our Solution

CommitMind aims to identify commitments from authorized source material, extract relevant details, and help users prioritize and follow through on their responsibilities.

## ✨ Key Features

- **Commitment Detection:** Identify potential commitments in text and conversations.
- **Deadline Extraction:** Find deadlines associated with commitments.
- **Ownership Tracking:** Identify the responsible person, with confirmation when uncertain.
- **Smart Prioritization:** Organize actions based on urgency and context.
- **Source Traceability:** Keep commitments linked to their original source for verification.
- **Follow-up Reminders:** Help users track pending and overdue responsibilities.

*Feature availability depends on the current prototype implementation.*

## 🛠️ Technology Stack

The project dependencies include:

- **Frontend:** React 19
- **Language:** TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS 4
- **AI SDK:** Google Gemini SDK (`@google/genai`)
- **Backend Dependencies:** Node.js and Express.js
- **Icons:** Lucide React
- **Animations:** Motion

The presence of a dependency does not necessarily mean its functionality is implemented or active in the current prototype.

## 🏗️ Proposed Architecture

1. **Ingest:** Process authorized emails, documents, or meeting notes.
2. **Extract:** Identify potential commitments using AI and natural language processing.
3. **Structure:** Extract the action, owner, deadline, and source.
4. **Verify:** Let users review uncertain information.
5. **Follow Through:** Prioritize actions and track progress.

The architecture is proposed; integrations and capabilities should be verified against the working implementation.

## 🚀 Getting Started

### Prerequisites

- Node.js
- npm
- A Google Gemini API key, if required by the implemented AI functionality

### Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/CommitMind.git
cd CommitMind
```

Install dependencies:

```bash
npm install
```

Configure environment variables according to `.env.example`, if applicable. Never commit API keys or other secrets.

Start the development server using the script defined in `package.json`:

```bash
npm run dev
```

## 🔐 Trust and Privacy

CommitMind's proposed design emphasizes:

- Explicit authorization for source access
- Least-privilege permissions
- Data minimization and retention controls
- Human verification of uncertain commitments
- Appropriate protection of sensitive information

These are design principles, not claims that every safeguard is already implemented.

## 👥 Team KERNEL

- **Adhayan Chanchal**
- **Shubham Agarwal**
- **Kenisha**
- **Shaurya**

**Institution:** Lloyd Institute of Engineering and Technology

## 🎯 Project Status

Hackathon MVP / prototype.

CommitMind is being developed to explore how AI can help people turn promises into accountable, actionable work.

---

**Every promise deserves a follow-through.**
