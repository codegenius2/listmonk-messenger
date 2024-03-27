<a href="https://zerodha.tech"><img src="https://zerodha.tech/static/images/github-badge.svg" align="right" /></a>

## listmonk-messenger

Lightweight HTTP server to handle webhooks from [listmonk](https://listmonk.app) and forward it to different messengers.

### Supported messengers

- Pinpoint
- Twilio
- AWS SES - Use `listmonk >= v2.2.0`


### Development

- Build binary

```
make build
```

- Change config.toml and tweak messenger config

Run the binary which starts a server on :8082

```
./listmonk-messenger.bin --config config.toml --msgr pinpoint --msgr ses
```

- Setting up webhooks
  ![](/screenshots/listmonk-setting-up-webhook.png)

- Add messenger specific subscriber atrributes in listmonk
  ![](/screenshots/listmonk-add-subsriber-attrib.png)

- Add plain text template
  ![](/screenshots/listmonk-plain-text-template.png)

- Change campaign messenger
  ![](/screenshots/listmonk-change-campaign-mgr.png)
