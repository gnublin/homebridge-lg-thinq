## If you using `homebridge-config-ui-x`

It's easy to grant access, go to plugin setting, select `Login with LG Account (plain username/password)` if you using LG account or select `Login with other methods` if you using 3rd-party like Google Account, Apple ID, Facebook ...

![](https://user-images.githubusercontent.com/54855446/132935957-917aafff-ef74-4af0-a367-207359b58cd8.png)

## if you using Hoobs and LG account

Put your `username` and `password` to plugin setting and it's done.

## if you using Hoobs and logged by Google account or Apple ID or Facebook account

I RECOMMENDED you to create new LG account (not logged by 3rd-party provider) and migrate all device to new account, it's fastest

or try following command in terminal

```
$ npm install -g homebridge-lg-thinq

$ thinq auth -c US -l en-US
Log in here: xxxxxx <- visit this url and select Google or Apple ID to login
Then paste the URL where the browser is redirected: <- then paste redirected url here

Your refresh_token: <- your refresh_token will be displayed here
```
