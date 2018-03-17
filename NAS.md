```sh
ssh admin@nas.wangcongyang.com -p 222
3#


docker create --name=calibre-web --restart=always \
-v /volume1/homes/admin/Calibre:/books \
-v /etc/localtime:/etc/localtime:ro \
-e PGID=65539 -e PUID=1029 \
-p 8083:8083 \
technosoft2000/calibre-web
```