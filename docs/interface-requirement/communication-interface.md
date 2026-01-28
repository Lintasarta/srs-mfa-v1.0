# Communication Interface

The following communication interfaces will be utilized:

- **HTTPS/TLS:** All communication between the user's web browser, the ai.cloudeka.id service portal, and any backend authentication services will be secured using HTTPS with TLS encryption to protect sensitive authentication data.

- **Internal API Endpoints:** New or modified internal API endpoints will be exposed to handle:
  - MFA enrollment (QR code generation, setup key provisioning).
  - MFA code verification during login.
  - MFA status updates (activation, deactivation).
  - MFA new code enrollment.

- **SMTP (for Email Authentication Fallback):** The system will use SMTP to send verification emails for the email authentication fallback mechanism.

- **User Interface (Web-based):** The primary communication interface for users will be the web-based service portal. This includes:
  - Login pages with MFA input fields.
  - "My Profile" section with MFA management options (e.g., slider for activation, password prompt, QR code display, input for security code).
  - Alert notification displays for invalid codes or other MFA-related messages.
