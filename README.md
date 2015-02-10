# Usage

## Run Container
```
docker run -d --restart always --name minidlna -p 8200:8200 -p 1900:1900/udp -v LOCAL_MEDIA_DIR:/opt rushcut/minidlna
```

or

```
docker run -d --restart always --name minidlna --net host -v LOCAL_MEDIA_DIR:/opt rushcut/minidlna
```


## Copy default conf to local

```
docker cp minidlna:/minidlna.conf /etc/mindlna/minidlna.conf
docker run -d --restart always --name minidlna --net host -v /etc/minidlna/minidlna.conf:/etc/minidlna/minidlna.conf -v LOCAL_MEDIA_DIR:/opt rushcut/minidlna
```

