# BudgetNest

![BudgetNest Logo](docs/logo.png)

https://github.com/Tokoloho17/Budget-Nest


BudgetNest is a personal finance management app that helps users log expenses, set goals, and stay motivated through gamified rewards and financial tips. Designed with simplicity and motivation in mind, BudgetNest is your companion on the journey to smarter money habits.

Application was coded and compiled by:
 Sendzo Matooane ST10369554
 Tichafara Zimudzi ST10365028
 Thembani Ngobeni ST10312968
 Tokoloho Hlalele ST10262724
---

## Features

- Sign Up & Login (Firebase Auth)
- Add & Categorize Expenses
- Rewards & Badge Unlocking
- Charts for Expense Trends (MPAndroidChart)
- Budget Goals
- View Expense History
- Motivational Tips on Rewards Screen


##Part 1: Research, Planning, and Design
Status: Completed
Deliverables:
•	Comparative research on three finance apps
•	Identification of strengths, weaknesses & features to adopt
•	Design of BudgeNest features & user experience
•	Wireframes and high-fidelity mockups
•	Gantt chart and project plan
•	Documented testing and deployment approach
Files: OPSC6311 POE Part 1 Research, OPSC6311 POE Part 1 Planning And Design
Part 2: Development Phase
Status: Completed
Individual Tasks Recap:
Tichafara (Tich) – Authentication & User Management
•	Firebase Authentication with email/Google
•	User login/signup UI
•	Basic user profile structure
•	Secured Firebase access via rules
Sendzo – Expense & Budget Management
•	Add, edit, delete expense entries
•	Create and manage budget goals
•	Firebase integration for storing expense and goal data
Teekay (Tokoloho) – Expense Tracking & Viewing
•	UI to display and filter expenses
•	Display category-wise spending
•	Graph integration for visual analysis (bridging Part 3)
Thembani – Local Storage & RoomDB
•	RoomDB for offline expense and goal data
•	Data sync logic between RoomDB and Firebase
•	Persistence across sessions
Part 3 / Final: Features, Visuals, and Firebase Completion
Status: Completed
Tasks Recap:
Person 1 – Graph UI & Goal Overlay
•	MPAndroidChart integrated
•	Category-wise expense graph
•	Min/Max goal overlays
•	Dynamic graph refresh on data change
•	Filters for week/month/custom ranges
•	Legends, tooltips, accessibility features
Person 2 – Goal Progress & Firebase Management
•	Visual dashboard with color-coded goal tracking
•	Firebase Firestore setup for all data (entries, goals, badges)
•	Firebase Authentication finalised
•	Firebase rules implemented
Person 3 – Gamification (Badges, Rewards)
•	Badge logic implemented (Daily Logger, Budget Master)
•	Firebase badge tracking with timestamps
•	GridView to show unlocked badges
•	(Optional) Sound or animation on unlock (if included)
Person 4 – Custom Features, Assets, and Documentation
•	Expense Reminders (daily notification at 7 PM)
•	Motivational Quotes module
•	App icon, splash screen, category & badge icons added
---

## Tech Stack

- Kotlin + Android Jetpack
- Firebase (Auth, Firestore, Realtime DB)
- Room (optional) for local storage
- MPAndroidChart for graphing
- ViewBinding for safe and clean UI code

---

## Folder Structure (Key Packages)

```
com.example.budgetnest
├── ui                  // All Activities (e.g. RewardsActivity, AddExpenseActivity)
├── data                // BadgeManager, BadgeDataSource
├── model               // Badge.kt, Expense.kt
├── auth                // LoginActivity, SignUpActivity
```

---

## Rewards System

The app rewards users with badges:

- Daily Logger – Log expenses for 7 days straight
- Budget Master – Stay within your budget all month

Each badge has a name, description, icon, and unlock status, managed through a `BadgeManager` and `BadgeDataSource`.

---

## Motivational Quotes

Displayed randomly on the Rewards screen:

> “Don’t save what is left after spending — spend what is left after saving.”  
> “Budgeting is telling your money where to go instead of wondering where it went.”

---

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/BudgetNest.git
   ```

2. Open in Android Studio:
   - File > Open > Select the project directory

3. Configure Firebase:
   - Add `google-services.json` to `app/` directory
   - Ensure Firebase is set up for Authentication and Firestore

4. Build APK:
   - Build > Build Bundle(s)/APK(s) > Build APK(s)
   - APK Location: `app/build/outputs/apk/debug/app-debug.apk`

---

## Release APK

To generate a signed APK:

1. Go to Build > Generate Signed Bundle / APK  
2. Choose APK > Select/Create a Keystore  
3. Set build type as release  
4. Finish to generate APK in:  
   `app/build/outputs/apk/release/app-release.apk`

---

## Future Improvements

- Export expenses to PDF/CSV  
- Notifications for daily tracking  
- More achievement badges  
- Dark mode toggle  
- Expense search & filters

---

## Author

Created by the BudgetNest Development Team

Feel free to contribute by opening pull requests or reporting issues!

---

## License

This project is licensed under the [MIT License](LICENSE).


