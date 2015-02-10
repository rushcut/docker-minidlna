# Usage

## Run Container
```
docker run -d --restart always --name minidlna -p 8200:8200 -p 1900:1900/udp -v /etc/minidlna:/etc/minidlna -v /data:/minidlna-data rushcut/minidlna
```

## Copy default conf to local
```
docker cp minidlna:/minidlna.conf /etc/mindlna/minidlna.conf
```
