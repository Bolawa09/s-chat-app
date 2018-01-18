## SimpleChat.Support - Open Source Live Chat App

- [https://www.simplechat.support](https://www.simplechat.support)

sChat (or SimpleChat or SimpleChat.Support) is an open source and very basic live chat app written by a JavaScript/Meteor developer. It is free and MIT licensed. You can use it in a SaaS-like model on the website or you can also create your own self-hosted copy of the app.

### Local run

- `git clone https://github.com/juliancwirko/s-chat-app.git`
- `cd s-chat-app`
- `npm install`
- `meteor --settings settings.json` (read more below)

### Documentation

- [https://www.simplechat.support/docs](https://www.simplechat.support/docs)

**Important:** Remember about Meteor settings file. The contents should look like:

```javascript
{
    "public": {
        "hostName": "localhost:3000 (or your-host-name.com in the prod)",
        "maxClientApps": 3,
        "maxChatHistoryInDays": 3,
        "ga": {
            "account": "UA-********-*" (your google analitics code - optional)
        }
    },
    "private": {
        "mainAppEmail": "your-email-address@gmail.com",
        "mailGun": "smtp://{Default SMTP Login}:{Default Password}@{SMTP Hostname}:587",
        "google": {
            "clientId": "{your google API client id here}",
            "secret": "{your google API secret key here}"
        },
        "facebook": {
            "appId": "{your facebook API app id here}",
            "secret": "{your facebook API secret key here}"
        }
    }
}
```

Read more about it here: [https://www.simplechat.support/docs#self-hosted-option](https://www.simplechat.support/docs#self-hosted-option)

### Changelog

- [CHANGELOG.md](https://github.com/juliancwirko/s-chat-app/blob/master/CHANGELOG.md)

### Contact

- julian.cwirko@gmail.com
- [Twitter - @juliancwirko](https://twitter.com/JulianCwirko)

### License

MIT

<a class="bmc-button" target="_blank" href="https://www.buymeacoffee.com/juliancwirko"><img src="https://www.buymeacoffee.com/assets/img/BMC-btn-logo.svg" alt=""><span style="margin-left:5px">Buy me a beer!</span></a>
