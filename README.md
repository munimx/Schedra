```markdown
# 📅 Schedra

Schedra is a **university timetable extractor** mobile application with offline caching.  
- **Backend**: .NET 8 Web API  
- **Frontend**: React Native (Android & iOS)  

The app extracts timetables, caches them locally, and automatically refreshes in the background when internet is available. Login credentials are stored securely so users don’t need to re-enter them every time.

---

## 🚀 Features
- Login once, stay signed in (secure credential storage).
- View cached timetable instantly offline.
- Automatic background refresh when internet is available.
- Cross-platform mobile support (Android & iOS).
- Scalable backend with clean architecture.

---

## 📂 Project Structure
```

Schedra/
│── backend/            # .NET 8 backend
│   ├── Schedra.Api/    # API project (controllers, services)
│   ├── Schedra.Core/   # Core business logic
│   ├── Schedra.Data/   # Data access (EF Core, persistence)
│   └── Schedra.Tests/  # Unit + integration tests
│
│── mobile/             # React Native mobile app
│   ├── android/        # Android native project
│   ├── ios/            # iOS native project
│   ├── src/            # App source code
│   │   ├── api/        # API client
│   │   ├── components/ # Shared UI components
│   │   ├── hooks/      # Custom hooks
│   │   ├── screens/    # Timetable, Login, Settings
│   │   └── utils/      # Helpers
│   └── App.tsx         # App entry point
│
│── .gitignore
│── README.md
│── schedra.sln

````

---

## ⚙️ Setup Instructions

### Prerequisites
- [Node.js](https://nodejs.org/) (>= 18)
- [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)
- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download)
- Xcode (for iOS dev, Mac only)
- Android Studio (for Android emulator/tools)

---

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/schedra.git
cd schedra
````

---

### 2. Backend Setup (.NET 8)

```bash
cd backend/Schedra.Api
dotnet restore
dotnet run
```

By default, API runs at `http://localhost:5000`.

---

### 3. Mobile Setup (React Native)

```bash
cd mobile
npm install
```

Run on iOS:

```bash
npx react-native run-ios
```

Run on Android:

```bash
npx react-native run-android
```

---

## 🔐 Environment Variables

Create a `.env` file in both `backend/` and `mobile/` as needed.
Example `.env.example` (root level):

```
# Backend
ASPNETCORE_ENVIRONMENT=Development
DB_CONNECTION_STRING=your-database-connection

# Mobile
API_BASE_URL=http://localhost:5000
```

---

## 🧪 Testing

### Backend

```bash
cd backend/Schedra.Tests
dotnet test
```

### Mobile (Jest/Unit Tests)

```bash
cd mobile
npm test
```

---

## 📦 Tech Stack

* **Backend**: .NET 8, C#, Entity Framework Core
* **Frontend**: React Native, TypeScript, AsyncStorage, Keychain
* **Database**: SQL Server / PostgreSQL (configurable)
* **Dev Tools**: VS Code, Xcode, Android Studio

---

## 📜 License

MIT License © 2025 Schedra

```
```
