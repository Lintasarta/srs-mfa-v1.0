# Product Features

The MFA enhancement will introduce the following key features:

## a. MFA Enrollment and Activation

- **User-Initiated MFA Activation (User Admin):** User Admins will have the ability to activate MFA for their accounts via a dedicated slider within their "My Profile" tab.
- **Super Admin-Initiated MFA Activation (User Admin):** Super Admins can activate MFA for User Admins through the "Manage Organization > More > Detail" menu. This action will enforce MFA on the User Admin's next login.
- **Password Confirmation for MFA Changes:** Any attempt to activate, deactivate, or re-enroll MFA will require the user to input their valid password for confirmation.
- **QR Code Provisioning:** Upon initiating MFA activation, the system will generate a QR code for users to scan with their authenticator applications (e.g., Google Authenticator, Microsoft Authenticator).
- **Setup Key Provisioning:** As an alternative to QR code scanning, a setup key will be provided for manual entry into authenticator applications.
- **Initial Security Code Verification:** After scanning the QR code or entering the setup key, users will be required to input a valid 6-digit security code from their authenticator app to complete the MFA setup.

## b. MFA Login Enforcement

- **TOTP Verification:** Users with active MFA will be prompted to enter a 6-digit security code from their authenticator application during login.
- **Email Authentication Fallback:** If a TOTP security code is unavailable (e.g., due to authenticator app issues), users can opt to use email authentication as a fallback method for login. This method is automatically triggered during the service portal onboarding process.
- **Invalid Code Handling:** The system will validate the provided security code, and an alert notification ("Invalid authentication code. Make sure the code is correct and not expired." or "Invalid or expired OTP") will be displayed for incorrect or expired codes.

## c. MFA Management

- **MFA Deactivation (User Admin):** User Admins will be able to deactivate MFA for their accounts via the "My Profile" tab (requires password confirmation).
- **Super Admin-Initiated MFA Deactivation (User Admin):** Super Admins can deactivate MFA for User Admins through the "Manage Organization > More > Detail" menu. This action will revert the User Admin's login to TOTP/Email Auth verification on their next login.
- **Enroll New MFA Code:** Both Super Admins and User Admins can enroll a new MFA code (e.g., when changing devices) via the "My Profile" section. This process involves password confirmation, QR code/setup key provisioning, and security code verification.
- **Administrative Scope:** Super Admin's ability to manage User Admin's MFA status is specifically within the "Manage Organization > More > Detail" menu, as the "Manage User" menu is for project access management only.

## d. User Experience

- **Clear Prompts and Notifications:** The system will provide clear on-screen instructions for MFA setup, login, and error handling.
- **Alert Messages:** Appropriate alert notifications will be displayed for invalid or expired authentication codes.
