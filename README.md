# CommitMind — AI-Powered Commitment Intelligence

> **Turning scattered promises into clear, actionable responsibilities.**  
> Every promise deserves a follow-through.

CommitMind is a proposed AI-powered commitment intelligence platform designed to identify promises and responsibilities hidden in authorized emails, documents, and meeting notes. It aims to turn them into reviewable action items with an owner, deadline, source evidence, priority, and follow-up reminders.

Unlike a conventional task manager that depends on someone manually creating a task, CommitMind focuses on finding the commitment at its origin: the conversation or document where it was made.

## The Problem

Important commitments are often buried in everyday communication:

- “I’ll send the report by Friday.”
- “Let’s follow up with the client next week.”
- “Please complete the task before the review.”

When these commitments remain scattered across different sources, people can lose track of ownership, deadlines, and follow-ups. Traditional reminders often begin only after someone has already created a task.

## The Proposed Solution

CommitMind adds a commitment-intelligence layer between communication and task management.

### Proposed workflow

1. **Ingest** — Accept authorized emails, documents, and meeting notes.
2. **Identify** — Use AI and natural-language processing (NLP) to detect possible commitments.
3. **Extract** — Identify the action, possible owner, deadline, source, and confidence.
4. **Confirm** — Ask the user to review unclear or uncertain details before creating an actionable commitment.
5. **Follow through** — Present prioritized actions, status tracking, and follow-up reminders.

### Proposed capabilities

- Commitment detection from text
- Owner and deadline extraction
- Source-linked evidence for verification
- Priority-based action dashboard
- Smart reminders and overdue alerts
- Follow-up suggestions and status tracking
- Team accountability with appropriate permissions

## Example Use Case

**Input message**

> “Could you send the revised proposal to Priya by Friday?”

**Possible extracted commitment**

| Field | Example |
|---|---|
| Action | Send the revised proposal |
| Owner | To be confirmed |
| Deadline | Friday; exact date may need confirmation |
| Source | Original email or message |
| Next action | Review the proposal and send it before the deadline |

This is an illustrative example, not a claim of measured product performance. CommitMind should ask for confirmation when ownership, dates, or meaning are ambiguous.

## Proposed Technology Stack

The pitch deck proposes the following stack. Final implementation choices may change as the MVP evolves.

| Layer | Proposed technology |
|---|---|
| Frontend | React or Next.js |
| Backend/API | Python with FastAPI |
| AI | LLM API with structured outputs |
| NLP | Text preprocessing and entity extraction |
| Database | PostgreSQL |
| Integrations | Gmail/Google Workspace or Microsoft 365 APIs, subject to authorization |
| Notifications | Email or in-app alerts |

## System Architecture

```text
Authorized Emails / Documents / Meeting Notes
                    |
                    v
              Text Extraction
                    |
                    v
         NLP / LLM Commitment Detection
                    |
                    v
       Extract Action, Owner, Deadline, Source
                    |
                    v
          Human Review & Confirmation
                    |
                    v
          Commitment / Task Database
                    |
                    v
       Priorities, Status, and Notifications
```

**Important design principle:** uncertain owners or deadlines should be flagged for review rather than silently assumed. Each commitment should retain a path back to its source so the user can verify the extracted information.

## Trust, Privacy, and Safety

CommitMind is designed around a human-confirmation checkpoint and privacy-conscious data handling.

Proposed principles include:

- **Explicit authorization:** Connect only accounts and sources the user has authorized.
- **Least-privilege access:** Request only the permissions needed for the selected features.
- **Data minimization:** Collect and retain only the data necessary for the product's purpose.
- **User verification:** Let users review and correct extracted commitments.
- **Uncertainty handling:** Flag unclear owners, deadlines, and interpretations.
- **Responsible model use:** Do not use sensitive user data to train models without appropriate authorization.

These are intended product principles; the implemented controls should be verified in the deployed application.

## Project Status

**Stage:** Hackathon MVP concept / proposed system.

The pitch deck describes the product vision, workflow, capabilities, architecture, and proposed technology stack. Features, integrations, and security controls should be treated as implemented only when they are present and tested in the repository.

## Getting Started

Setup instructions depend on the code currently in the repository. Once the frontend, backend, and environment configuration are finalized, add the exact installation and run commands here.

Typical setup documentation should cover:

1. Prerequisites and supported versions
2. Cloning the repository
3. Installing frontend and backend dependencies
4. Configuring environment variables
5. Setting up the database
6. Starting the application
7. Running tests

### Environment variables

Do not commit API keys, access tokens, passwords, or other secrets to GitHub. Document required variable **names** in an `.env.example` file and keep the actual `.env` file out of version control.

## Roadmap

- [ ] Build the initial web interface
- [ ] Implement text input and ingestion for authorized sources
- [ ] Add commitment detection and structured extraction
- [ ] Add source evidence and confidence/uncertainty handling
- [ ] Implement human review and confirmation
- [ ] Store confirmed commitments in PostgreSQL
- [ ] Add priorities, status tracking, and reminders
- [ ] Evaluate extraction quality using representative test cases
- [ ] Add authorized email/calendar integrations
- [ ] Test access controls, privacy, and failure cases

Roadmap items are planned work, not statements that these features are already complete.

## Team

**Team KERNEL**  
Lloyd Institute of Engineering and Technology

- Adhyayan Chanchal
- Shubham Agarwal
- Kenisha
- Shaurya

## Why CommitMind?

Task managers organize tasks people already know they need to create. CommitMind aims to identify the promise behind the task, preserve its source, and help people move from conversation to accountable follow-through.

## Contributing

Contributions, suggestions, and feedback are welcome. If you plan to contribute, describe the issue or proposed change first, then submit a pull request with a clear explanation and relevant tests.

## License

No license has been specified yet. Until a license is added to this repository, do not assume that the code is available for reuse, redistribution, or modification. Consider adding an appropriate open-source license before inviting external contributions.

---

*CommitMind — Every promise deserves a follow-through.*
