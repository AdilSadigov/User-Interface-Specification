# User Management Screen UI Specification

## Overview
The User Management screen is composed of a navigation bar (navbar) at the top and a main area divided into two sections. 

## Navbar
The navbar hosts three components:
1. `New User` button
2. `Save User` button
3. `Hide Disabled User` checkbox

### 1. `New User` Button
- **Location**: Left side of the navbar.
- **Purpose**: To create a new user.
- **Color**: Blue.

### 2. `Save User` Button
- **Location**: Right side of the navbar.
- **Purpose**: To save the added user details into the user table.
- **Color**: Blue.

### 3. `Hide Disabled User` Checkbox
- **Location**: To the right of the `New User` button.
- **Purpose**: To hide disabled users in the user table when checked.

## Main Area
The main area is divided into two parts:
1. Existing user table
2. New user form

### 1. Existing User Table
- **Location**: Left side of the main area.
- **Columns**: It contains four columns named ID, User Name, Email, Enabled. The column names are in the same color as the navbar buttons.

### 2. New User Form
- **Location**: Right side of the main area.
- **Title**: "New User" at the top, indicating the purpose of this area.
- **Input Fields**: It includes four input fields named User Name, Display Name, Phone, Email.
- **User Roles Dropdown**: A dropdown list with three options - Guest, Admin, SuperAdmin.
- **Enabled Checkbox**: To choose if the user is enabled or not.

When all fields are filled, the `Save User` button in the navbar should be clicked to save the user data into the user table.

## Behavior
- Clicking on the `New User` button will clear all the fields in the new user form and prepare it for new user data input.
- The `Save User` button should only be active if all the mandatory fields in the form are filled out.
- After saving the user data using the `Save User` button, the new user details will be added to the table in the left section of the main area.
- Checking the `Hide Disabled User` checkbox will hide all the users with an 'Enabled' status of 'false' in the user table.
- Unchecking the `Hide Disabled User` checkbox will reveal all the users regardless of their 'Enabled' status.
