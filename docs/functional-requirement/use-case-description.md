# Use Case Description

**Action and Response**

| Action by user | Response from system |
|---|---|
| *Super Admin Login with Valid QR Code for MFA Enforcement* | *Super Admin successfully logs in with MFA Enforcement. MFA Status becomes: Active.* |
| *Super Admin Login with Valid Setup Key for MFA Enforcement* | *Super Admin successfully logs in with MFA Enforcement. MFA Status becomes: Active. Super Admin can use TOTP for subsequent logins as long as the Security Code is available on the Authenticator. Super Admin can use Email Auth for subsequent logins if the Security Code is unavailable on the Authenticator.* |
| *User Admin Login with Valid QR Code for MFA Enforcement* | *User Admin successfully logs in with MFA Enforcement. MFA Status becomes: Active. User Admin can use TOTP for subsequent logins as long as the Security Code is available on the Authenticator. User Admin can use Email Auth for subsequent logins if the Security Code is unavailable on the Authenticator.* |
| *User Admin Login with Valid Setup Key for MFA Enforcement* | *User Admin successfully logs in with MFA Enforcement. MFA Status becomes: Active. User Admin can use TOTP for subsequent logins as long as the Security Code is available on the Authenticator. User Admin can use Email Auth for subsequent logins if the Security Code is unavailable on the Authenticator.* |
| *Super Admin Login with Valid TOTP (Non-MFA Enforcement)* | *Super Admin successfully logs in using TOTP Verification.* |
| *Super Admin Login with Valid Email Authentication (Non-MFA Enforcement)* | *Super Admin successfully logs in using Email Authentication.* |
| *User Admin Login with Valid TOTP (Non-MFA Enforcement)* | *User Admin successfully logs in using TOTP Verification.* |
| *User Admin Login with Valid Email Authentication (Non-MFA Enforcement)* | *User Admin successfully logs in using Email Authentication.* |
| *Super Admin Enrolls MFA New Code with Valid QR Code* | *Super Admin successfully Enrolls New Code. An alert notification appears: "A New Multi-Factor Authentication has been successfully enrolled".* |
| *Super Admin Enrolls MFA New Code with Valid Setup Key* | *Super Admin successfully Enrolls New Code. An alert notification appears: "A New Multi-Factor Authentication has been successfully enrolled".* |
| *User Admin Enrolls MFA New Code with Valid QR Code* | *User Admin successfully Enrolls New Code. An alert notification appears: "A New Multi-Factor Authentication has been successfully enrolled".* |
| *User Admin Enrolls MFA New Code with Valid Setup Key* | *User Admin successfully Enrolls New Code. An alert notification appears: "A New Multi-Factor Authentication has been successfully enrolled".* |
