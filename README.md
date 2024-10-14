
# Finance Tracking App

## Project Abstract

The **Finance Tracking App** is a cross-platform mobile application built using **React Native** that allows users to manage their personal finances. Users can track their income, expenses, set budgets for different categories, and visualize their spending patterns through intuitive charts. The app helps users gain control over their financial health by providing clear overviews of their budget progress and expense history.

---

## High-Level Concept

This app enables users to:
- Add, view, and delete transactions (income/expenses).
- Categorize transactions (e.g., food, rent, transport, etc.).
- Set and track budgets for each category.
- View visual summaries (charts) to analyze spending trends.
- Optionally, log in and save their financial data using cloud storage like Firebase.

The app is developed using **React Native**, which allows for seamless deployment on both Android and iOS. It will use local storage for offline use and provide data synchronization features through a cloud backend if needed.

---

## Tools and Libraries

### Core Tools
1. **React Native** – Framework for building cross-platform mobile applications.
2. **Expo** – To simplify React Native development and manage native dependencies.
3. **AsyncStorage** – For local storage to persist user data offline.
4. **Firebase** (optional) – For user authentication and cloud storage.
5. **Victory Native / Recharts** – For data visualization (e.g., expense charts).
6. **React Navigation** – For navigation between screens.

### UI/UX Libraries
1. **React Native Paper** or **NativeBase** – For pre-built UI components (cards, buttons, etc.).
2. **React Native Vector Icons** – For icons throughout the app.
3. **Styled Components** or **CSS-in-JS** – For styling the app.

---

## Project Checklist

### 1. Project Setup
- [x] Initialize a new React Native project using **Expo**.
  ```bash
  npx create-expo-app finance-tracker-app
  cd finance-tracker-app
  npm start  # or yarn start
  ```

- [ ] Install dependencies for navigation and storage:
  ```bash
  npm install @react-navigation/native @react-navigation/stack
  expo install react-native-screens react-native-safe-area-context
  expo install @react-native-async-storage/async-storage
  ```

- [ ] Install UI libraries:
  ```bash
  npm install react-native-paper react-native-vector-icons
  ```

- [ ] Install charting library:
  ```bash
  npm install victory-native
  ```

### 2. Basic Structure
- [ ] Setup **React Navigation** for screen routing.
  - Create navigation for **Dashboard**, **Transactions**, **Add Transaction**, and **Settings** screens.
- [ ] Create a **Dashboard** that shows balance, recent transactions, and budget progress.
- [ ] Setup state management using **useState** or **useReducer** for handling transactions.

### 3. Transaction Management
- [ ] Create a screen to **Add Transactions** (income or expense).
- [ ] Implement a **Transaction List** that shows all transactions.
- [ ] Implement features to **Edit** and **Delete** transactions.

### 4. Budget Tracking
- [ ] Allow users to **set a budget** for specific categories (e.g., groceries, rent, transport).
- [ ] Show budget progress using a **progress bar** or **circular gauge**.
- [ ] Notify users when they are nearing the budget limit.

### 5. Data Persistence
- [ ] Use **AsyncStorage** to persist user data (transactions, budget) locally on the device.
- [ ] Implement functions to **save and retrieve** data from AsyncStorage.
- [ ] Add a **Clear Data** option in settings to reset all data.

### 6. Data Visualization
- [ ] Use **Victory Native** to display charts.
  - Show a **Pie Chart** for expense breakdown by category.
  - Display a **Line Graph** for tracking expenses over time.
- [ ] Ensure charts update dynamically as transactions are added or removed.

### 7. Optional Features
- [ ] Integrate **Firebase** for user authentication and cloud storage of transactions.
- [ ] Implement push notifications using **Expo Notifications** to remind users of upcoming bills or budget limits.
- [ ] Add **multi-currency** support, allowing users to select their preferred currency.
- [ ] Implement **offline mode**, allowing users to use the app without an internet connection and sync data when online.

---

## App Folder Structure
```plaintext
src/
  components/
    TransactionList.js        # List of all transactions
    TransactionItem.js        # Single transaction component
    AddTransactionForm.js     # Form for adding new transactions
    BudgetProgress.js         # Budget progress bar
  screens/
    DashboardScreen.js        # Main dashboard screen
    TransactionsScreen.js     # View and manage all transactions
    AddTransactionScreen.js   # Screen to add new transactions
    SettingsScreen.js         # App settings (currency, reset data)
  services/
    auth.js                   # Firebase or other authentication services
    database.js               # Local/Cloud database handling (AsyncStorage or Firebase)
  utils/
    formatDate.js             # Utility for formatting dates
    currencyFormatter.js      # Utility for formatting currencies
```

---

## Steps for Development

### 1. Initial Setup
- Create your screens (`DashboardScreen`, `TransactionsScreen`, etc.).
- Set up navigation using **React Navigation** to switch between these screens.
- Install and configure necessary libraries (AsyncStorage, React Native Paper, Victory Native, etc.).

### 2. Build Core Features
- Start with the **Dashboard** and display the current balance, total income, and expenses.
- Build out the **Add Transaction Form** and implement functionality to add transactions to your state.
- Create the **Transaction List** and allow users to view, edit, or delete transactions.

### 3. State Management
- Use **useState** or **useReducer** to manage transactions and budgets in the app.
- Ensure that state is persistent by saving and retrieving data from **AsyncStorage**.

### 4. Build Visualizations
- Add data visualization to the dashboard using **Victory Native**.
- Display a pie chart for expense breakdown and a line chart for expenses over time.

### 5. Test and Improve
- Test the app on both Android and iOS using Expo.
- Debug and ensure all features (transactions, budgets, charts) work as expected.
- Test the app offline and ensure data persists.

---

## Future Improvements
- Implement **user authentication** with Firebase to save user data in the cloud.
- Add **push notifications** to remind users of bills or budget thresholds.
- Integrate additional features like **multi-currency support** or a **dark mode**.

---

## Resources and Documentation
- [React Native Documentation](https://reactnative.dev/docs/getting-started)
- [Expo Documentation](https://docs.expo.dev/)
- [React Navigation](https://reactnavigation.org/)
- [Victory Native for Charts](https://formidable.com/open-source/victory/docs/native/)
- [AsyncStorage Documentation](https://react-native-async-storage.github.io/async-storage/docs/usage/)
- [Firebase Authentication](https://firebase.google.com/docs/auth)
- [Expo Notifications](https://docs.expo.dev/versions/latest/sdk/notifications/)

---
