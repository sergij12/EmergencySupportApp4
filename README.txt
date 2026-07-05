EmergencySupportApp
===================

Що це:
- готовий MVP-проєкт для Android Studio
- Kotlin + Jetpack Compose + Room + DataStore
- персональні плани дій, ресурси, чек-лист, довідник, режим тривоги

Як відкрити:
1. Розпакуй ZIP.
2. В Android Studio натисни Open і вибери папку EmergencySupportApp.
3. Дочекайся Gradle Sync.
4. Запусти на емуляторі.

Важливо:
- У цьому середовищі я не зміг додати файл gradle-wrapper.jar, бо немає доступу до мережі.
- Якщо Android Studio попросить Gradle Wrapper, найпростіше створити будь-який новий Empty Compose Project і перенести в нього папки app, build.gradle.kts, settings.gradle.kts, gradle.properties.
- Вся логіка та код проєкту вже всередині.

Що реалізовано:
- Onboarding
- Home
- Resources
- Planner
- Alarm mode
- Guide
- Checklist
- Local storage через Room
