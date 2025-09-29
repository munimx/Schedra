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

## 📦 Tech Stack

* **Backend**: .NET 8, C#, Entity Framework Core
* **Frontend**: React Native, TypeScript, AsyncStorage, Keychain
* **Database**: SQL Server / PostgreSQL (configurable)
* **Dev Tools**: VS Code, Xcode, Android Studio
```
````
