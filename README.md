# 🆘 Emergency Support — Android app with an AI assistant

An Android app that helps people prepare for emergencies: personal action plans, a supply checklist, a reference guide, an alarm mode and an AI assistant powered by **Google Gemini**.

<!-- Add 3–4 phone screenshots side by side -->
<!-- <img src="docs/home.png" width="220"> <img src="docs/ai.png" width="220"> -->

## Features

- 🤖 **AI assistant (Gemini)** — chat that answers questions and generates a personal emergency plan
- 📋 **Planner** — step-by-step action plans for different emergency types
- ✅ **Checklist** — supplies and documents to prepare
- 📚 **Guide** — offline reference information
- 🚨 **Alarm mode** — quick access to the most important actions
- 👤 **Onboarding, profile and sign-in**
- 💾 **Works offline** — data stored locally in Room and DataStore

## Tech stack

- **Kotlin**, **Jetpack Compose**, Material 3
- **MVVM** (ViewModel + Repository), Kotlin Coroutines
- **Room** (local database), **DataStore** (settings)
- **Navigation Compose**
- **Google Gemini API**
- minSdk 24, targetSdk 34

## Project structure

```
com/example/emergencysupport/
├── data/
│   ├── ai/          # Gemini assistant
│   ├── local/       # Room database, DAOs, entities
│   ├── repository/  # repositories
│   └── seed/        # initial data
└── ui/
    ├── screen/      # home, planner, checklist, guide, alarm, ai, profile…
    ├── component/   # reusable Compose components
    ├── navigation/
    └── viewmodel/
```

## Run

1. Open the project in Android Studio and wait for Gradle sync.
2. Add your Gemini key to `local.properties` (see `local.properties.example`):
   ```
   GEMINI_API_KEY=your_key_here
   ```
3. Run on an emulator or a device.

The API key is read at build time and is never committed to the repository.

## Author

Sergij — Android, front-end and automation developer. Open to freelance projects.
