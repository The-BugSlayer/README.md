# README.md
# Fintech App Test Cases

This document contains structured test case scenarios for a **Fintech Application**, covering authentication, transactions, security, and notifications.

## 1. User Authentication

### ✅ Successful Login
- **Steps:**
  1. Enter valid email/phone number and password.
  2. Click **Login**.
  3. Verify user is redirected to the dashboard.

### ❌ Invalid Credentials
- **Steps:**
  1. Enter incorrect email/phone or password.
  2. Click **Login**.
  3. Verify error message: **"Invalid credentials"** appears.

### 🔐 Two-Factor Authentication (2FA)
- **Steps:**
  1. Enable 2FA in settings.
  2. Attempt login.
  3. Verify OTP is sent via SMS/email.
  4. Enter the OTP and confirm login.

---

## 2. Fund Transfers

### ✅ Successful Transfer
- **Steps:**
  1. Enter recipient’s account number.
  2. Input amount within balance limit.
  3. Click **Send** and enter transaction PIN.
  4. Verify transaction success message appears.

### ❌ Insufficient Funds
- **Steps:**
  1. Enter amount exceeding account balance.
  2. Click **Send**.
  3. Verify error message: **"Insufficient funds"** appears.

### 🔄 Cancel Pending Transfer
- **Steps:**
  1. Initiate a transfer.
  2. Before confirmation, click **Cancel**.
  3. Verify transaction is not processed.

---

## 3. Bill Payments

### ✅ Successful Bill Payment
- **Steps:**
  1. Select biller (e.g., DSTV, PHCN, MTN).
  2. Enter customer details and amount.
  3. Click **Pay**.
  4. Verify payment success message.

### ❌ Invalid Biller Details
- **Steps:**
  1. Enter incorrect biller details.
  2. Click **Pay**.
  3. Verify error message **"Invalid account details"** appears.

---

## 4. Card Management

### ✅ Create Virtual Card
- **Steps:**
  1. Go to **Cards** section.
  2. Click **Create Virtual Card**.
  3. Enter funding source and amount.
  4. Verify card is created and displayed.

### ❌ Network Failure During Card Creation
- **Steps:**
  1. Initiate card creation.
  2. Simulate network disruption.
  3. Verify error message **"Network error, try again"** appears.

---

## 5. Security & Fraud Prevention

### 🔐 Lock Debit Card
- **Steps:**
  1. Go to **Card Settings**.
  2. Click **Lock Card**.
  3. Verify card cannot be used for transactions.

### 🔄 Report Unauthorized Transactions
- **Steps:**
  1. Go to **Transaction History**.
  2. Select a suspicious transaction.
  3. Click **Report Issue**.
  4. Verify support team receives the complaint.

---

## 🔹 6. Notifications & Alerts

### ✅ Transaction Alert
- **Steps:**
  1. Complete a transaction.
  2. Verify user gets a push notification and SMS/email alert.

### 🔄 OTP Not Received
- **Steps:**
  1. Initiate a transaction requiring OTP.
  2. Simulate a network failure.
  3. Verify **"OTP not received?"** option is displayed.

---

📌 **Contributors:** Feel free to add more test cases or report issues! 🚀
