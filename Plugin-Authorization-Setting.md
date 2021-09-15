## If you using `homebridge-config-ui-x`

It's easy to grant access, go to plugin setting, select `Login with LG Account (plain username/password)` if you using LG account or select `Login with other methods` if you using 3rd-party like Google Account, Apple ID, Facebook ...

![](https://user-images.githubusercontent.com/54855446/132935957-917aafff-ef74-4af0-a367-207359b58cd8.png)

## if you using Hoobs and LG account

Put your `username` and `password` to plugin setting and it's done.

## if you using Hoobs and logged by Google account or Apple ID or Facebook account

I RECOMMENDED you to create new LG account (not logged by 3rd-party provider) and migrate all device to new account, it's fastest

or you can install `homebridge-config-ui-x` to use Custom UI feature

or you can try below guide to manual obtain `refresh_token`

* look at this url: `https://us.m.lgaccount.com/spx/login/signIn?client_id=LGAO221A02&svc_list=SVC202&svc_integrated=Y&redirect_uri=https%3A%2F%2Fvn.m.lgaccount.com%2Flogin%2FiabClose&show_thirdparty_login=LGE%2CMYLG%2CGGL%2CAMZ%2CFBK%2CAPPL&division=ha&callback_url=https%3A%2F%2Fvn.m.lgaccount.com%2Flogin%2FiabClose&oauth2State=12345&show_select_country=N`
* change `redirect_uri` and `callback_url` param value to your country code url `[your country code].m.lgaccount.com`
* visit modified url, then select your 3rd-party login type
* when logged successfully, you may redirected to blank page, don't worry, just copy that URL and you can find refresh_token in this URL, it will look like `https://us.m.lgaccount.com/spx/login/iabClose?access_token=*******&refresh_token=***this is what you need***&oauth2_backend_url=https://us.lgeapi.com/`
* then you put `refresh_token` to plugin setting