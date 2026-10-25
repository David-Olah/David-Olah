# David Olah

Software engineer working on full-stack web and mobile applications and applied machine learning. I take projects through to production, with tests, CI, and hosting in place, so they're ready for real users. Below is a selection of that work.

## Publication

### [Recycling Catalytic Converters for Sustainable Resource Management](https://dl.acm.org/doi/10.1145/3715335.3735462)

*Lead author, ACM Digital Library*

The paper presents an image classification system that categorizes catalytic converters to support recycling and resource recovery. I designed the training pipeline and evaluation for a siamese network approach, which reached 95% classification accuracy.

## Selected Projects

### [Quartermaster](https://github.com/David-Olah/Quartermaster-showcase)

A tool tracking platform for construction companies. Every tool carries a QR label that crews scan from their phones to check it out to a jobsite or return it, while managers track location, holders, overdue items, damage flags, and upcoming maintenance.

- Multi-tenant REST API, React Native mobile app for iOS and Android, and a React admin web app
- Offline check-outs and check-ins that queue on the device and sync on reconnect
- Shared zod schemas across all three apps, so an API change surfaces as a type error in every client
- Transactional conflict checks on reservations to prevent double-booking, with role permissions enforced in the API

**Stack:** TypeScript, Express 5, Prisma, PostgreSQL, React Native (Expo), React, Vite

[Live demo](https://app.quartermastersite.com)

### [Lorekeeper](https://github.com/David-Olah/Lorekeeper-showcase)

A campaign wiki for tabletop RPG groups that publishes directly from an Obsidian vault. It enforces per-user visibility: the game master's private notes stay private, each player keeps personal notes on every page, and shared group notes sync in real time.

**Stack:** React, Node.js, Express, PostgreSQL, WebSockets, TypeScript (Obsidian plugin)

[Live demo](https://lorekeeper-my6h.onrender.com/c/the-ashen-vale-demo)

### [YinshAI](https://github.com/David-Olah/Yinsh_AI)

A model that predicts the winner of a game of Yinsh from a mid-game board state. I wrote a parser for Boardspace.net game records spanning 2006 to 2023, reconstructed each game's board states into a 2D representation, and trained an XGBoost classifier on the result. The model reaches 71.2%
