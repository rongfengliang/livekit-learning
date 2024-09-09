# livekit 部署测试

```code
Note: --node-ip needs to be reachable by the client. 127.0.0.1 is accessible only to the current machine

Server URL:  ws://localhost:7880
API Key: APISQ9nphM6rhbq
API Secret: gJ3bwaXiLbO9Y8QvtXXgCmi1lkf23HpUHmqdg0HwW7J
```

## token gen

```code
lk  token create --api-key APISQ9nphM6rhbq --api-secret gJ3bwaXiLbO9Y8QvtXXgCmi1lkf23HpUHmqdg0HwW7J   --join --room my-first-room   --identity  demo --name demo --valid-for  1000h

lk  token create   --api-key APISQ9nphM6rhbq --api-secret gJ3bwaXiLbO9Y8QvtXXgCmi1lkf23HpUHmqdg0HwW7J  --join --room mydemov6   --identity  demo --name demo  --valid-for  1000h
```


## load test

```code
lk load-test  --url ws://localhost:7880 --api-key APISQ9nphM6rhbq --api-secret gJ3bwaXiLbO9Y8QvtXXgCmi1lkf23HpUHmqdg0HwW7J --room  my-first-room --video-publishers 10 
```

## ingress

```code
lk  --url ws://localhost:7880 --api-key APISQ9nphM6rhbq --api-secret gJ3bwaXiLbO9Y8QvtXXgCmi1lkf23HpUHmqdg0HwW7J ingress create ingress.json
```

