## MSBot Integration
#### Installation
The easiest way to install this integration is to use KPM.
```sh
/kpm install msbot
```

#### Configuration
To add a configuration, execute each of the following commands (replace each of the angle bracketed strings with the respective information):
```sh
/kpm config msbot commandPrefix "!"
/kpm config msbot key "<path to TLS key, eg key.pem>"
/kpm config msbot cert "<path to TLS cert, eg cert.pem>"
/kpm config msbot app_id "<Microsoft App ID>"
/kpm config msbot app_secret_password "<Microsoft App Secret Password>"
/kpm config msbot port <port number>
```

#### Running
To run MSBot, either run `node main.js msbot` when starting Concierge or run `/kpm start msbot` when Concierge is running.

#### Notes
- To obtain a TLS certificate easily, the Lets Encrypt project has [easy ways of doing this](https://letsencrypt.org/getting-started/).
- Currently MSBots works on platforms supported [here](https://docs.botframework.com/en-us/csharp/builder/sdkreference/gettingstarted.html#channels).
- Port defaults to 8000.
- If using a service like ngrok, you do not need to supply a key or cert.
- To setup your bot register it [here](https://dev.botframework.com/bots/new).
