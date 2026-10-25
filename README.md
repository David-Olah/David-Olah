David Olah

Software engineer working on full-stack web and mobile applications and applied machine learning. I take projects through to production, with tests, CI, and hosting in place, so they're ready for real users. Below is a selection of that work.

Publication

Recycling Catalytic Converters for Sustainable Resource Management, ACM Digital Library. Lead author.

The paper presents an image classification system that categorizes catalytic converters to support recycling and resource recovery. I designed the training pipeline and evaluation for a siamese network approach, which reached 95% classification accuracy.

Selected projects

Quartermaster is a tool tracking platform for construction companies. Every tool carries a QR label that crews scan from their phones to check it out to a jobsite or return it, while managers track location, holders, overdue items, damage flags, and upcoming maintenance. It consists of a multi-tenant REST API (Express 5, Prisma, PostgreSQL), a React Native mobile app for iOS and Android, and a React admin web app. The mobile app queues check-outs and check-ins while offline and syncs them on reconnect. Request and response schemas are shared zod types across all three apps, so an API change surfaces as a type error in every client. Reservations use transactional conflict checks to prevent double-booking, and role permissions are enforced in the API. The admin app is live with a demo company.

Lorekeeper is a campaign wiki for tabletop RPG groups that publishes directly from an Obsidian vault. It enforces per-user visibility: the game master's private notes stay private, each player keeps personal notes on every page, and shared group notes sync in real time over WebSockets. Built with React, Node.js, Express, and PostgreSQL, with an Obsidian plugin written in TypeScript. Live demo.

YinshAI predicts the winner of a game of Yinsh from a mid-game board state. I wrote a parser for Boardspace.net game records spanning 2006 to 2023, reconstructed each game's board states into a 2D representation, and trained an XGBoost classifier on the result. The model reaches 71.2% accuracy, and the project includes an analysis of how prediction accuracy changes by turn.
