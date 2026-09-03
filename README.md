# 🕌 Muslim Connect

Muslim Connect is a full-stack mobile application designed to help Muslims organize important aspects of their spiritual, financial, and community lives in one platform.

The application combines spiritual practices, financial commitments, charitable activities, and community-oriented features to help users manage their responsibilities with greater peace of mind.

## 📱 About the Project

Muslim Connect provides a centralized platform for managing different aspects of everyday Muslim life, including:

* 🕌 Spiritual practices and acts of worship
* 💰 Debts, loans, and financial commitments
* 🤲 Charitable contributions
* 📊 Installment and remaining-balance tracking
* 📜 Shared wills
* 🕊️ Bereavement-related features
* 🕌 Salat al-Janaza
* 👥 Community-oriented functionality
* 🔔 Push notifications

The project follows a **mobile-to-backend architecture**, with a Flutter application communicating with a Symfony REST API.

---

## ✨ Key Features

### 🕌 Spiritual & Community Features

Muslim Connect provides features designed to support users in organizing spiritual responsibilities and participating in community-oriented activities.

### 💰 Financial Commitment Management

Users can manage different types of financial obligations, including:

* Debts
* Loans
* Amanas
* Installments
* Payment status
* Remaining balances

The system supports installment-based payments and automatically tracks the remaining amount of an obligation.

### 🔔 Notifications

The application integrates push notifications to keep users informed about important events and updates.

### 🔐 Authentication

The backend provides secure authentication using JWT-based authentication.

---

## 🏗️ Architecture

```text
┌──────────────────────────────┐
│       Flutter Mobile App     │
│                              │
│   UI · Navigation · Services │
└──────────────┬───────────────┘
               │
               │ REST API
               │ JWT Authentication
               ▼
┌──────────────────────────────┐
│       Symfony Backend        │
│                              │
│ Controllers · Services       │
│ Business Logic · API         │
└──────────────┬───────────────┘
               │
               │ Doctrine ORM
               ▼
┌──────────────────────────────┐
│          Database            │
└──────────────────────────────┘

               │
               ▼

        Firebase Services
   Push Notifications · Storage
```

---

## 🛠️ Tech Stack

### Frontend

* Flutter
* Dart
* Firebase
* REST API integration

### Backend

* Symfony
* PHP
* Doctrine ORM
* JWT Authentication
* REST API

### Database

* MySQL / PostgreSQL

### Additional Tools & Services

* Firebase Cloud Messaging
* Firebase Storage
* Git
* GitHub
* Postman

---

## 📂 Project Structure

```text
Muslim-Connect/
│
├── backend/                  # Symfony REST API
│   ├── config/
│   ├── migrations/
│   ├── src/
│   │   ├── Controller/
│   │   ├── Entity/
│   │   ├── Repository/
│   │   └── Service/
│   ├── templates/
│   └── composer.json
│
├── frontend/                 # Flutter mobile application
│   ├── android/
│   ├── ios/
│   ├── assets/
│   ├── lib/
│   │   ├── models/
│   │   ├── services/
│   │   └── ui/
│   └── pubspec.yaml
│
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

* Flutter SDK
* Dart
* PHP
* Composer
* Symfony CLI
* MySQL or PostgreSQL
* Git

---

## 🔧 Backend Setup

```bash
cd backend
```

Install PHP dependencies:

```bash
composer install
```

Configure your environment variables locally.

Create your local environment configuration without committing credentials to Git.

Run database migrations:

```bash
php bin/console doctrine:migrations:migrate
```

Start the Symfony server:

```bash
symfony server:start
```

---

## 📱 Frontend Setup

Navigate to the frontend:

```bash
cd frontend
```

Install dependencies:

```bash
flutter pub get
```

Run the application:

```bash
flutter run
```

> If you run the Flutter application on an Android emulator, the backend running on your local machine may be accessible through `10.0.2.2`.

---

## 🔐 Security

Sensitive files and local configuration are intentionally excluded from version control.

Examples include:

```text
.env
.env.*
key.properties
*.jks
*.keystore
*.pem
*.key
google-services.json
GoogleService-Info.plist
```

Never commit production credentials, private keys, signing keys, Firebase credentials, API keys, or environment-specific secrets.

---

## 🧠 What I Worked On

This project allowed me to work across both mobile and backend development, including:

* Building a Flutter mobile application
* Developing REST APIs with Symfony
* Implementing JWT authentication
* Designing database entities and relationships
* Managing financial obligations and installment logic
* Integrating Firebase services
* Implementing push notifications
* Connecting the mobile application to backend APIs
* Managing project version control with Git and GitHub

---

## 🔮 Future Improvements

Potential improvements include:

* Improved automated testing
* CI/CD pipeline
* Dockerized development environment
* Enhanced API documentation
* Improved notification management
* Expanded community features
* Additional analytics and reporting
* Production deployment configuration

---

## 📸 Screenshots

Screenshots and application previews can be added here.

```text
Coming soon
```

---

## 👨‍💻 Author

**Ali Balti**

Full-Stack & Mobile Developer

* GitHub: https://github.com/Alibalti592
* Portfolio: https://ali-balti-portfolio-3x2k.bolt.host/

---

## 📄 License

This project is currently intended for portfolio and demonstration purposes.

---

⭐ If you found this project interesting, feel free to explore the code and follow the repository.
