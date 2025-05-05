
# MERN Fullstack Starter Template

A modern and minimal boilerplate to kickstart your fullstack web development using **MongoDB**, **Express**, **React**, and **Node.js** — complete with linting, formatting, Git hooks, and environment configuration.

---

## 📦 Tech Stack

- **MongoDB** – NoSQL database
- **Express.js** – Node.js web framework
- **React** – Frontend library (CRA or Vite-based)
- **Node.js** – Backend runtime
- **ESLint + Prettier** – Code quality and formatting
- **Husky + lint-staged** – Git pre-commit hooks
- **dotenv** – Environment variables

---

## 🧰 Folder Structure

project-root/
├── backend/ # Express server files
│ └── server.js
├── frontend/ # React application (empty until you install React)
├── .husky/ # Git hooks
├── .gitignore # Ignore files
├── .eslintrc.json # ESLint configuration
├── .prettierrc # Prettier configuration
├── package.json # Root scripts and devDeps
└── README.md # You’re reading it now


---

## 🚀 Getting Started

### 1. Clone the Template

```bash
git clone https://github.com/your-username/mern-template-project.git your-project-name
cd your-project-name

2. Install Dependencies
npm install
This installs all root, backend, and dev dependencies — including ESLint, Prettier, Husky, etc.

🧪 React Setup (Frontend)
cd frontend
npx create-react-app . --template cra
# or use Vite:
# npm create vite@latest . -- --template react
npm install

🌐 MongoDB Setup
1. Create a .env in the root:
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/<dbname>?retryWrites=true&w=majority

2.  Add .env to .gitignore (already done in this template).

✅ Pre-Commit Linting
This template uses Husky + lint-staged to format and lint code before every commit.

If you cloned the template and initialized Git yourself:
git init
npm run prepare
npx husky install
After that, Git hooks will work on commit.


⚙️ Scripts

"scripts": {
  "dev": "nodemon backend/server.js",
  "prepare": "husky install",
  "lint": "eslint .",
  "format": "prettier --write ."
}

npm run dev - Start the backend server

npm run lint - Check code issues

npm run format - Format code using Prettier

🛡️ .gitignore Included


This template includes a comprehensive .gitignore that covers:

Node

React

MongoDB

Lint caches

OS junk files

Build outputs

CI tools

Monorepos

and more

👥 Contributing
Feel free to fork this template and adapt it to your needs. PRs welcome if you find bugs or want to suggest improvements.

