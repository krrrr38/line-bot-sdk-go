# golang echo - LINE Messaging API

Sample echo-bot

## Getting started local env

```
$ export CHANNEL_SECRET=YOUR_LINE_CHANNEL_SECRET
$ export CHANNEL_TOKEN=YOUR_LINE_CHANNEL_ACCESS_TOKEN

$ go get -u github.com/line/line-bot-sdk-go/linebot
$ go run main.go
```

## Getting started with Heroku

### heruku button

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/krrrr38/line-bot-sdk-go)

then set Webhook URL: `https://{YOUR_APP}.herokuapp.com/callback`

### deploy by yourself

```sh
heroku create
heroku info # then set Webhook URL: https://{YOUR_APP}.herokuapp.com/callback
heroku config:set CHANNEL_SECRET="..."
heroku config:set CHANNEL_TOKEN="..."
git push heroku master
heroku logs
```
