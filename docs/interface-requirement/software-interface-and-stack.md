# Software Interface and Stack

The MFA enhancement for the ai.cloudeka.id service portal will interact with the following key software components:

- **Existing Authentication System (ai.cloudeka.id):** The MFA module will integrate with the current email verification-based authentication system to add a second factor of authentication. This includes:
  - **Login Flow:** Intercepting the login process after initial credential validation to prompt for MFA.
  - **User Management:** Accessing user data (e.g., email, roles) to determine MFA enforcement policies and to associate MFA configurations with user accounts.
  - **"My Profile" Section:** Modifying the existing "My Profile" user interface to include MFA activation/deactivation and new code enrollment functionalities.

- **Authenticator Applications:**
  - **Google Authenticator:** The system will generate QR codes and setup keys compatible with Google Authenticator for TOTP generation.
  - **Microsoft Authenticator:** The system will generate QR codes and provide manual entry options compatible with Microsoft Authenticator.
  - **Other TOTP-compatible Authenticator Apps:** While specifically mentioning Google and Microsoft Authenticator, the implementation should adhere to standard TOTP protocols to support other compatible authenticator applications.
