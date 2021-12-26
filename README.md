# zenbot-helm

This repository enables deployment of [zenbot](https://github.com/DeviaVir/zenbot) on a kubernetes cluster using helm.

## General procedure

1. Add the repo to helm
```
helm repo add zenbot https://larsac.github.io/zenbot-helm/
```

1. Install a release
```
helm install zenbot zenbot/zenbot
```

## Deployment parameters
Check out the following options or refer to `values.yaml` for more details.

|Parameter|Default|Comment|
|---------|-------|-------|
|zenbot.binance_api_key|none|Provide your Binance API key|
|zenbot.binance_secret|none|Provide your Binance API secret|
|zenbot.ifttt_enable|true|Whether to enable notifications via IFTTT|
|zenbot.ifttt_api_key|none|IFTTT API key|

