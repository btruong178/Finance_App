
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
