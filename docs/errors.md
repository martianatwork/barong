# Barong errors list

## Resource module errors
```
resource.labels.private   -                 Can't update Label.
resource.user.no_activity                   No activity recorded or wrong topic
resource.profile.not_exist                  User has no profile
resource.profile.exist                      Profile already exists
resource.api_key.2fa_disabled               Only accounts with enabled 2FA alowed
resource.api_key.missing_otp                Theaccount has enabled 2FA but OTP code is missing
resource.api_key.invalid_otp                OTP code is invalid
resource.phone.twillio                      Something wrong with Twilio Client
resource.phone.invalid_num                  Phone number is invalid
resource.phone.number_exist                 Phone number already exists
resource.phone.verification_invalid         Phone is not found or verification code is invalid
resource.documents.limit_reached            Maximum number of documents already reached
resource.documents.limit_will_be_reached    Documents amount will reach limit by this upload
resource.otp.already_enabled                2FA has been already enabled for this account
resource.otp.invalid                        OTP code is invalid
resource.password.doesnt_match              New passwords don\'t match
resource.password.prev_pass_not_correct     Previous password is not correct
resource.password.no_change_provided        New password cant be the same, as old one
```

## Identity module errors
```
identity.user.invalid_referral_format   Invalid referral uid format
identity.user.referral_doesnt_exist     Referral doesn't exist
identity.user.active_or_doesnt_exist    User doesn't exist or has already been activated'
identity.password.user_doesnt_exist     User doesn't exist
identity.user.passwords_doesnt_match    Passwords don't match
identity.user.utilized_token            JWT has already been used
identity.session.invalid_login_params   Invalid Email or Password
identity.session.invalid                Invalid Session
identity.captcha.required               captcha_response is required'
identity.captcha.mandatory_fields       Mandatory fields must be filled in
identity.session.not_active             Your account is not active
identity.session.banned                 Your account is banned
identity.session.invalid_params         Invalid Email or Password
identity.session.missing_otp            The account has enabled 2FA but OTP code is missing
identity.session.invalid_otp            OTP code is invalid
```

## Admin module errors
```
admin.user.update_himself    Admin can't update himself
admin.user.enable_2fa        Manual 2FA enabling not allowed
admin.user.state_no_change   Can't change state, as its already {active}
admin.user.doesnt_exist      User with such UID doesnt exist
admin.label.doesnt_exist     Label with such key doesnt exist or not assigned to chosen user
admin.access.denied          Access Denied: User is not Admin
admin.user.non_user_field    Search field is not a user attribute
admin.user.no_matches        Search result is empty array
```

## General errors
```
record.not_found                Record is not found
jwt.decode_and_verify           Failed to decode and verify JWT
authz.invalid_session           Failed to decode cookies
authz.user_not_active           User is not active
authz.invalid_signature         API Key header 'signature' is invalid
authz.apikey_not_active         API Key state is 'inactive'
authz.disabled_2fa              API Key owner has disabled 2FA
authz.invalid_api_key_headers   Blank or missing API Key headers
authz.permission_denied         Path is blacklisted
authz.unexistent_apikey         X-Auth-Apikey header is invalid
```