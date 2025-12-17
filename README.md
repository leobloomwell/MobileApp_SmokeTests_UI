# Bloomwell Mobile – Smoke Tests (Flutter, Android & iOS)

This repository contains automated **mobile smoke tests** for the Bloomwell Flutter application on **Android and iOS**.

The goal of this test suite is to verify that the most critical user flows work correctly after each deployment on **staging** and **production-like environments**.

---

## Technology Stack

- Flutter Integration Tests
- Dart
- Flutter `integration_test`
- Android Emulator / Physical Device
- iOS Simulator / Physical Device
- BrowserStack (optional)

---

## Test Scope (Smoke Level)

### 1. App Launch & Initialization
- Application starts without crashes
- Splash screen loads successfully
- Initial API calls complete

---

### 2. Authentication / Registration
- Registration screen opens
- Mandatory field validation works
- User can register using valid test data
- User can log in with an existing account
- Session is created successfully

---

### 3. Home & Navigation
- Home screen loads after login
- Bottom navigation tabs are visible
- Navigation between main sections works

---

### 4. Product Listing & Search
- Product list loads correctly
- Search returns results
- Wrapped and non-wrapped products are displayed when applicable

---

### 5. Order Flow (Smoke)
- Order creation can be started
- Pharmacy selection is visible
- Delivery method selection works
- Pick-up and delivery options render correctly

Note: Payment and deep order logic are covered by separate test suites.

---

### 6. Order Details
- Order details screen opens
- Pharmacy information is displayed
- “Rechnung” (invoice) link visibility is validated
- Pick-up address is displayed for pick-up orders

---

### 7. Platform & Feature Flag Validation
- Feature behavior is consistent between Android and iOS
- Same account behaves identically on both platforms
- Feature flag–dependent content is validated

---

## Platforms Covered

- Android (minimum supported version)
- Android 14 / 15 (latest)
- iOS (latest stable version)

Tests are executed on:
- Emulators / Simulators
- Physical devices
- BrowserStack devices (optional)

---

## Project Structure

