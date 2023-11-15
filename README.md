# mfa-layer
Add OTP token based MFA to any website, even if they don't support it

## Idea:

1. Create MFA app
2. MFA app creates email accounts itself
3. You give it your password
4. It also generates the usual OTP tokens
5. You register the email account only the MFA app has access to
6. Whenever you login to your website of choice, the MFA app requests a password reset
7. The new password will be your password + OTP token + some sort of secret only the MFA app has
8. Only if you give the MFA app the correct password can you generate an OTP taken that leads to the correct resetted password
9. There you go, MFA for any "password recovery email" account
