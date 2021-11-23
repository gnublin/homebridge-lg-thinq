## Grant access by LG account

This plugin use LG account with username/password to grant access

## If your account logged by Google account or Apple ID or Facebook account (using Third-party login)

You can create a second account with username/password, then assigning access to the home from the google/apple/facebook authenticated account to the new account.

Watch this video: https://www.youtube.com/watch?v=TIQU0Wo92E8

You can use same email with google/apple/facebook account, LG treats them as separate accounts.

Put your `username` and `password` of your second account to plugin setting and it's done.

## if you don't want to provide username/password, you can use `refresh_token` instead

following command in terminal to grant `refresh_token`

```
$ npm install -g homebridge-lg-thinq

$ thinq login [username] [password] -c US -l en-US <- correcting your account country and language

Your refresh_token: <- your refresh_token will be displayed here
```

put `refresh_token` to plugin setting