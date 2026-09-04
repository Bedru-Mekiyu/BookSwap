# BookSwap 📚🔁

[![Android CI](https://github.com/Bedru-Mekiyu/BookSwap/actions/workflows/android-ci.yml/badge.svg)](https://github.com/Bedru-Mekiyu/BookSwap/actions/workflows/android-ci.yml)
[![Kotlin](https://img.shields.io/badge/Kotlin-1.9.20-blue.svg?logo=kotlin)](https://kotlinlang.org/)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-brightgreen.svg?logo=android)](https://developer.android.com/jetpack/compose)
[![Material 3](https://img.shields.io/badge/Design-Material%203-7b2cbf.svg)](https://m3.material.io/)

BookSwap is a modern Android application designed for book lovers to seamlessly showcase, discover, and trade physical books within their community. Built with Kotlin and modern Android Jetpack libraries, BookSwap provides a intuitive interface for managing personal collections and arranging exchanges.

---

## 🚀 Key Features

* **User Authentication & Profiles**
  * Profile creation with custom preferences and preferred reading genres.
  * Account credential navigation for login and signup flows.

* **Book Management & Discovery**
  * Add books to personal exchange listings with title, author, genre, condition, and image resources.
  * Browse available books listed by community members.
  * Dedicated book details UI displaying condition, description, and owner contact details.

* **Swap & Trade Workflow**
  * Initiate exchange requests directly from book listings.
  * Propose counter-offers from personal collections.
  * Track active swap requests and status updates.

---

## 🛠️ Architecture & Tech Stack

* **Language**: Kotlin 1.9
* **UI Framework**: Jetpack Compose (Declarative UI)
* **Design System**: Material Design 3 (`androidx.compose.material3`)
* **Navigation**: Compose Navigation (`androidx.navigation.compose`)
* **Image Loading**: Coil Compose (`io.coil-kt:coil-compose`)
* **Build System**: Gradle with Kotlin DSL (`build.gradle.kts`)
* **Minimum SDK**: API 24 (Android 7.0)
* **Target SDK**: API 34 (Android 14)

---

## 📁 Project Structure

```text
BookSwap/
├── .github/
│   └── workflows/
│       └── android-ci.yml         # GitHub Actions CI build & test workflow
├── bookswap/
│   ├── app/
│   │   ├── src/
│   │   │   ├── main/
│   │   │   │   ├── java/com/example/bookswap/
│   │   │   │   │   ├── data/      # Data models and sample dataset
│   │   │   │   │   ├── screens/   # Jetpack Compose screen components (Home, AddBook, Profile, etc.)
│   │   │   │   │   ├── ui/theme/  # Material 3 colors, typography, and theme definitions
│   │   │   │   │   ├── MainActivity.kt
│   │   │   │   │   └── Navigation.kt
│   │   │   │   ├── res/           # Android resources (drawables, mipmaps, strings)
│   │   │   │   └── AndroidManifest.xml
│   │   │   └── test/              # Unit tests
│   │   ├── build.gradle.kts       # Module Gradle configuration
│   │   └── proguard-rules.pro
│   ├── build.gradle.kts           # Root Gradle configuration
│   ├── gradle.properties
│   ├── settings.gradle.kts
│   └── gradlew                    # Gradle wrapper script
└── README.md
```

---

## ⚡ Getting Started

### Prerequisites

* **Android Studio**: Jellyfish (2023.3.1) or newer recommended.
* **JDK**: Java 17 Development Kit.
* **Android SDK**: API Level 34 installed.

### Installation & Execution

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Bedru-Mekiyu/BookSwap.git
   cd BookSwap/bookswap
   ```

2. **Build the Debug APK**:
   ```bash
   ./gradlew assembleDebug
   ```

3. **Run Unit Tests**:
   ```bash
   ./gradlew test
   ```

---

## 🧪 CI/CD Workflow

Automated testing and build validation are handled via GitHub Actions in `.github/workflows/android-ci.yml`. On every `push` and `pull_request` to the main branch, CI executes:
1. Environment setup with JDK 17 (Temurin).
2. Dependency verification via Gradle cache.
3. Unit test suite execution (`./gradlew test`).
4. Debug build compilation (`./gradlew assembleDebug`).

---

## 👥 Authors & Contributors

| Member Name | ID |
| :--- | :--- |
| **Bedru Mekiyu** | UGR/7000/15 |
| **Tinsae Jembere** | UGR/7993/15 |
| **Tsedenya Bazezew** | UGR/9693/15 |
| **Bethelihem Wondimneh** | UGR/7686/15 |
| **Natnael Endale** | UGR/5583/15 |

---

## 📄 License

This project is available under standard repository terms.
