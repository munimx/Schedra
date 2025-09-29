```markdown
# 📅 Schedra

Schedra is a **university timetable extractor mobile application** with a **.NET 8.0 backend** and **React Native frontend**.  
It allows students to log in once, extract their timetable from the university portal, cache it locally, and view it even when offline.  

If the user is online, the app fetches updated data in the background and refreshes the cache seamlessly.  

---

## ✨ Features
- 🔐 Secure login with stored credentials (no need to re-enter every time).  
- 📂 Cached timetable for offline access.  
- 🌐 Background refresh when internet is available.  
- 📱 Mobile app built with React Native (Android + iOS).  
- ⚡ Backend powered by .NET 8.0 Web API.  

---

## 🗂 Project Structure
```

Schedra/
│── .gitignore
│── README.md
│── schedra.sln               # .NET solution file
│
├── backend/                  # .NET 8.0 Web API
│   ├── Schedra.Api/          # Main API project (Controllers, Services, Models)
│   ├── Schedra.Core/         # Business logic layer
│   ├── Schedra.Data/         # EF Core & database context
│   └── Schedra.Tests/        # Unit & integration tests
│
└── mobile/                   # React Native mobile app
├── android/              # Android-specific project files
├── ios/                  # iOS-specific project files
├── src/                  # App source code
│   ├── api/              # API client for backend communication
│   ├── components/       # Reusable UI components
│   ├── hooks/            # Custom React hooks (auth, cache, etc.)
│   ├── screens/          # App screens (Login, Timetable, Settings)
│   └── utils/            # Helpers & constants
└── App.tsx               # App entry point

````

---

## 🛠 Tech Stack
### Backend
- **.NET 8.0 Web API** – RESTful API layer  
- **Entity Framework Core** – ORM & database access  
- **xUnit** – Testing framework  

### Frontend
- **React Native 0.74** – Mobile application (iOS + Android)  
- **TypeScript** – Type safety and clean code  
- **AsyncStorage** – Offline caching  
- **react-native-keychain** – Secure credential storage  

### Infra / Tooling
- **Git & GitHub** – Version control  
- **VS Code** – Development environment  
- **Xcode / Android Studio** – For iOS and Android builds  
- **npm / Yarn** – Package management  

---

````

```

```
```
