# Currency-Converter
QuickConverter is an Android app designed to provide fast, accurate, and reliable currency conversions. It integrates the ExchangeRate.host API for real-time exchange rates and uses Firebase Realtime Database for offline storage, user preferences, and multi-device synchronization.

1. Project Links

GitHub Repository: https://github.com/Gudani12/CurrencyExchangeApp￼
Demonstration Video (YouTube): https://www.youtube.com/shorts/g3Zy7d1bCCc￼

⸻

2. Overview

The Currency Converter App (QuickConverter) is a fully functional Android application designed to help users convert between global currencies with live exchange rates. It supports user authentication, API integration, Firebase storage, offline functionality, and multilingual support.

This version implements all feedback from previous submissions and is prepared for deployment to the Google Play Store.

⸻

3. Purpose

The purpose of this app is to provide a reliable, real-time, and offline-capable currency conversion solution for users who need quick access to global exchange rates, secure login, and a personalized experience through saved settings and favorite currencies.

⸻

4. Key Features
	•	User Registration and Login (Encrypted Passwords)
	•	Single Sign-On (SSO) Integration
	•	Real-Time Exchange Rate Conversion using REST API
	•	Offline Mode with Firebase Sync
	•	Real-Time Notifications using Firebase Cloud Messaging
	•	Settings Management (Default Currency, Theme, etc.)
	•	Multi-language Support (English + Tshivenda)
	•	Push Notifications for Currency Alerts
	•	Modern MVVM Architecture with LiveData
	•	App Icon and Responsive UI Design

⸻

5. Technical Overview

API Integration
	•	Base URL: https://api.exchangerate.host
	•	Endpoints Used:
	•	/latest?base={currency} – Fetches the latest rates.
	•	/convert?from={currency}&to={currency}&amount={value} – Converts specific amounts.
	•	Data parsed using Retrofit for efficient network handling.

Firebase Integration
	•	Firebase Realtime Database: Stores user preferences, cached rates, and favorites.
	•	Firebase Cloud Messaging: Handles push notifications and real-time alerts.
	•	Offline Caching: Allows conversions without internet connectivity.

Database Design
	•	Users: ID, Email, Password, Preferred Currency
	•	Rates: Base Currency, Target Currency, Value, Timestamp
	•	Favorites: Saved Currencies

⸻

6. App Architecture

The project follows MVVM (Model-View-ViewModel) architecture:
	•	Model: Handles API and Firebase logic.
	•	ViewModel: Communicates between the model and UI.
	•	View: Reactively updates UI via LiveData.

This structure ensures testability, scalability, and clear separation of concerns.

⸻

7. Offline Mode & Sync

The app uses Firebase’s offline caching system, allowing users to convert currencies even without internet access. When the user reconnects, new exchange rates are automatically synchronized.

⸻

8. Real-Time Notifications

Using Firebase Cloud Messaging (FCM), users receive real-time updates and alerts about major currency rate changes or app notifications.

⸻

9. Multi-Language Support

The app supports two South African languages:
	•	English
	•	Zulu
    •   Afrikaans

Users can switch between languages in the settings screen.

⸻

10. Automated Testing & GitHub Actions

The repository includes GitHub Actions for automated builds and test validation to ensure:
	•	Successful build on each commit.
	•	Functional testing for key features.
	•	Tagging of final release as “Final POE”.

⸻

11. Release Notes

Version: 2.0 (Final POE Release)
Date: November 2025

Updates Since Prototype:
	•	Implemented Firebase offline sync.
	•	Added real-time push notifications.
	•	Introduced multi-language support.
	•	Enhanced UI responsiveness.
	•	Optimized API calls for better performance.
	•	Added app icon and publishing configurations.

⸻

12. Testing Summary
	•	Unit and Integration Tests completed successfully.
	•	Offline and online conversions tested with valid and invalid inputs.
	•	Firebase authentication and data sync confirmed functional.
	•	Push notifications tested on mobile device (Android).

All key tests passed successfully.

⸻

13. Evidence of Publication Preparation

(Space for screenshots showing signed APK, Play Console upload, and publishing steps.)

⸻

14. AI Tool Usage

ChatGPT was used to assist with documentation structure, code debugging, and improving readability of technical explanations. All generated content was reviewed, customized, and verified by the project team.

⸻

15. Conclusion

The Currency Converter App meets all required outcomes of the OPSC6312 module. It demonstrates proficiency in Android development, API integration, Firebase storage, push notifications, and multi-language implementation. The app is stable, user-friendly, and ready for Play Store publication.
