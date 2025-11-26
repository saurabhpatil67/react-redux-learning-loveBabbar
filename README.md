# React Redux Learning Repository

This repository contains my practice code from Love Babbar’s **React + Redux** lecture series.  
It includes all essential Redux concepts such as **actions, reducer slices, store, state, useSelector, useDispatch, and payload**.

---

## 🚀 Redux Concepts Covered

### 🔹 1. Action
- An **action** is a simple JavaScript object.
- It tells Redux **what happened**.
- Example: `{ type: "increment" }`

### 🔹 2. Reducer Slice (createSlice)
- A **slice** contains:
  - initial state  
  - reducers (functions that update state)  
  - actions generated automatically  
- It is created using `createSlice()` from Redux Toolkit.

### 🔹 3. Store
- The **store** is the single place where the entire app state is stored.
- Created using `configureStore()`.
- The store connects **reducers** and **UI (React)**.

### 🔹 4. State
- The **state** is the actual data stored in Redux.
- Example:  
  ```js
  { count: 0 }

---

## 📖 Terminology Dictionary

| Term | Simple Definition | The "Real World" Analogy |
| :--- | :--- | :--- |
| **Store** | The single source of truth. It holds the entire state tree of your application. | **The Bank Vault:** Where all the money (data) is kept secure. |
| **State** | The actual data currently living inside the store. | ** The Money:** The actual cash balance inside the vault at this moment. |
| **Slice** | A collection of Redux logic for a *single feature* (e.g., Counter, User, Cart). It contains the initial state, reducers, and actions. | **Department:** The "Loans Department" or "Savings Department" within the bank. |
| **Action** | An event that describes *something happened*. It has a `type` (name) and optional `payload` (data). | **Deposit Slip:** A form you fill out saying "I want to deposit" (type) "$50" (payload). |
| **Payload** | The specific data attached to an action that is needed to update the state. | **The $50 Bill:** The actual item you are handing over with your deposit slip. |
| **Reducer** | A function that takes the *current state* and an *action*, and decides how to update the state. | **The Bank Teller:** Takes your slip (action) and money (payload), and updates your account balance. |
| **Dispatch** | A function used to trigger an action. It sends the action to the store. | **Handing it over:** The physical act of giving the deposit slip to the teller. |
| **useSelector**| A hook to read data from the store. | **Checking Balance:** Looking at your bank app to see how much money you have. |
