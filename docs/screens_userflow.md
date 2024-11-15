# Screens and User Flow Documentation

## Overview
This document outlines all the screens in the messaging app, their purpose, functionality, and user flow.

---

## Screens

### 1. Splash Screen
- **Purpose**: Initial screen shown while the app loads.
- **Actions**:
  - Check if the user is logged in.
  - Redirect to the **Login** screen if not logged in, or to the **Home** screen if logged in.

---

### 2. Login Screen
- **Purpose**: Allows users to log in using their email and password.
- **Elements**:
  - Email input field.
  - Password input field.
  - Login button.
  - "Forgot Password?" link.
  - Sign-up link for new users.
- **Actions**:
  - Validate user credentials and redirect to the **Home** screen on success.

---

### 3. Registration Screen
- **Purpose**: Allows new users to create an account.
- **Elements**:
  - Email input field.
  - Password input field.
  - Confirm password field.
  - Sign-up button.
- **Actions**:
  - Register the user and send a verification email.
  - Redirect to the **Login** screen after successful registration.

---

### 4. Home Screen
- **Purpose**: Central hub of the app, displaying recent chats.
- **Elements**:
  - List of recent conversations with users and groups.
  - Floating action button (FAB) to start a new chat.
- **Actions**:
  - Tap on a chat to open the **Chat Screen**.

---

### 5. Chat Screen
- **Purpose**: Displays conversation history and allows users to send and receive messages.
- **Elements**:
  - Messages list (scrollable).
  - Input field for typing messages.
  - Send button.
  - Media attachment button.
- **Actions**:
  - Send text messages.
  - Attach and send media.

---

### 6. Contacts Screen
- **Purpose**: Displays a list of contacts who are also app users.
- **Elements**:
  - Search bar for filtering contacts.
  - Add new contact button.
- **Actions**:
  - Select a contact to open a new chat.

---

### 7. Profile Screen
- **Purpose**: Displays and allows editing of user profile information.
- **Elements**:
  - User's profile picture.
  - Name and email.
  - Edit button.
- **Actions**:
  - Update profile details.
  - Change profile picture.

---

### 8. Settings Screen
- **Purpose**: Allows users to configure app settings.
- **Elements**:
  - Notifications toggle.
  - Theme (light/dark mode) toggle.
  - Privacy settings.
- **Actions**:
  - Adjust settings and save changes.

---

### 9. Forgot Password Screen
- **Purpose**: Allows users to reset their password.
- **Elements**:
  - Email input field.
  - Reset button.
- **Actions**:
  - Send password reset email and redirect to the **Login** screen.

---

### 10. Media Viewer Screen
- **Purpose**: Displays media (images, videos) in full-screen mode.
- **Elements**:
  - Media preview.
  - Download button.
  - Share button.
- **Actions**:
  - View, download, or share media.

---

## User Flow

### User Login Flow
#### Description
Guides users through the login process from the splash screen to the home screen.

![User Login Flow](./uml/User%20Login%20Flow.svg)

---

### User Registration Flow
#### Description
Guides new users through the account creation process.

![User Registration Flow](./uml/User%20Registration%20Flow.svg)

---

### Messaging Flow
#### Description
Covers sending and receiving messages in the chat screen.

![Messaging Flow](./uml/Messaging%20Flow.svg)

---

### Password Reset Flow
#### Description
Outlines the process of resetting a user's password.

![Password Reset Flow](./uml/Password%20Reset%20Flow.svg)

---

### Contact Addition Flow
#### Description
Covers adding a new contact to the user's contact list.

![Contact Addition Flow](./uml/Contact%20Addition%20Flow.svg)

---

## Notes for Designers
1. Ensure all screens follow a consistent visual theme.
2. Maintain clear visual hierarchy to highlight important actions (e.g., FABs, primary buttons).
3. Include user feedback for actions (e.g., loading indicators, success/error messages).
4. Optimize for accessibility:
   - Use high-contrast colors.
   - Support screen readers.
   - Provide large tappable areas for buttons.

---
