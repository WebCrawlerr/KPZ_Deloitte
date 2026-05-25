# KPZ_Deloitte – Prompt Management Application (DeloiHub)
Hackers don't code, they write prompts.
The application allows for the creation, versioning, and sharing of prompts in a cloud environment. The project was built using React + Vite and AWS Amplify, ensuring scalability and ease of deployment.

## 📦 Technologies
**Frontend:** React + Vite + TypeScript

**Backend:** AWS Amplify (Cognito, AppSync, DynamoDB)

**Hosting:** AWS Amplify Hosting

**State Management:** React Context API

## 🚀 Features
✅ Creating and editing prompts

📜 Version history with the ability to compare changes

👥 Sharing prompts with other users

🔐 Authorization and authentication via Amazon Cognito

☁️ Cloud deployment on AWS Amplify

## 🛠️ Installation and Local Setup
Clone the repository:
```bash
git clone [https://github.com/IwoStaykov/KPZ_Deloitte.git](https://github.com/IwoStaykov/KPZ_Deloitte.git)
cd KPZ_Deloitte
```

Install dependencies:
```bash
npm install
```

Run the application:
```bash
npm run dev
```

The application will be available at: http://localhost:5173

## 🌐 Cloud Deployment (AWS Amplify)
The project is integrated with AWS Amplify, enabling easy deployment and scalability of the application. The `amplify.yml` file contains the CI/CD pipeline configuration.

To deploy the application:

1. Log in to the AWS Amplify Console.
2. Connect your GitHub repository and select the `dev` branch.
3. Amplify will automatically build and deploy the application.

## 📁 Project Structure
```csharp
KPZ_Deloitte/
├── amplify/            # AWS Amplify configuration
├── public/             # Static files
├── src/                # Application source code
│   ├── components/     # React components
│   ├── pages/          # Application pages
│   ├── types/          # TypeScript type definitions
│   └── App.tsx         # Main application component
├── amplify.yml         # Amplify CI/CD configuration
├── package.json        # Project dependencies
└── README.md           # Project documentation
```

## 🤝 Repository Structure and Workflow Guidelines

In our repository, we have adopted an organized branching model based on the Git Flow approach. This makes it easier for us to develop the application, test new features, and maintain stability on the main production branch.

### 📌 Main Branches
* **`main`**
The primary production branch. Only stable, tested code goes here.
Changes can only be integrated into `main` via pull requests from `dev`.

* **`dev`**
The integration branch where we test new features. All completed features are merged here before being released to production.

### 🌱 Working Branches
* **`feature/feature-name`**
New features are developed on separate branches starting with `feature/`, which branch off from `dev`.
Once the work is completed and merged into `dev`, the branch can be deleted.

* **`fix/fix-name`**
Hotfix branches for `main`, used if a bug occurs in the production environment despite the testing process.
These branches should also be integrated and deleted as quickly as possible once the work is completed.
