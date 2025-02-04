# Campus Navigator

## Introduction  
Campus Navigator is a mobile application designed to help students, staff, and visitors navigate university campuses with real-time indoor/outdoor directions.

## Getting Started  

### Prerequisites  
- **Git**: [Install Git](https://git-scm.com/)  
- **Node.js** (v16+): [Install Node.js](https://nodejs.org/)  
- **Expo CLI** (for frontend):  
  ```bash
  npm install -g expo-cli
  ```

### Installation  
1. **Clone the repository**:  
   ```bash
   git clone https://github.com/zayeemZaki/campus-navigator.git
   cd campus-navigator
   ```

2. **Switch to the `develop` branch**:  
   ```bash
   git checkout develop
   ```

---

## Project Setup  

### Frontend (React Native)  
**Folder**: `frontend`  
1. Navigate to the frontend directory:  
   ```bash
   cd frontend
   ```
2. Install dependencies:  
   ```bash
   npm install
   ```
3. **Environment Setup**:  
   - Create a `.env` file in the `frontend` folder:  
     ```bash
     touch .env
     ```
   - Add your Mapbox API key:  
     ```plaintext
     MAPBOX_ACCESS_TOKEN=your_mapbox_token_here
     ```
4. Start the development server:  
   ```bash
   npm start
   ```

### Backend (Node.js/Express)  
**Folder**: `backend`  
1. Navigate to the backend directory:  
   ```bash
   cd backend
   ```
2. Install dependencies:  
   ```bash
   npm install
   ```
3. **Environment Setup**:  
   - Create a `.env` file in the `backend` folder:  
     ```bash
     touch .env
     ```
   - Add Firebase credentials (ask the team lead for keys):  
     ```plaintext
     FIREBASE_PROJECT_ID=your_project_id
     FIREBASE_CLIENT_EMAIL=your_client_email
     FIREBASE_PRIVATE_KEY=your_private_key
     ```
4. Start the server:  
   ```bash
   npm run dev
   ```

---

## Branch Management  

### Workflow  
- **`main`**: Stable, production-ready code.  
- **`develop`**: Active development branch. All PRs should target this branch.  

### Creating a Feature Branch  
1. Always create a new branch for your work:  
   ```bash
   git checkout -b feature/your-feature-name
   ```
   Example:  
   ```bash
   git checkout -b feature/add-indoor-navigation
   ```

2. Push your branch to GitHub:  
   ```bash
   git push -u origin feature/your-feature-name
   ```

### Submitting Changes  
1. Commit with a descriptive message:  
   ```bash
   git commit -m "feat: add indoor navigation logic"
   ```
2. Create a **Pull Request (PR)** on GitHub:  
   - Target the `develop` branch.  
   - Tag `@zayeemZaki` or other reviewers.  

### Syncing with `develop`  
To avoid conflicts, regularly pull the latest changes:  
```bash
git checkout develop
git pull origin develop
```

---

## Contributing Guidelines  
1. **Code Style**: Follow existing patterns and use ESLint/Prettier.  
2. **Testing**: Write unit tests for new features (e.g., `npm test`).  
3. **Documentation**: Update the README or wiki for major changes.  
4. **Issues**: Report bugs via GitHub Issues with the `bug` label.  

---

## Troubleshooting  
- **Dependency Issues**: Delete `node_modules` and run `npm install`.  
- **Mapbox Errors**: Verify your `.env` file has the correct API key.  
- **Firebase Auth**: Ensure service account keys are added to `backend/.env`.  

---

## License  
This project is licensed under the [MIT License](LICENSE).  
```
