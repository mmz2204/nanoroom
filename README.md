# Nano cluster example

## About this example



## How to run the example?

```shell
cd examples/customerroute
go build
peer
# run master server
./customerroute master
./customerroute chat --listen "127.0.0.1:34580"
./customerroute chat --listen "127.0.0.1:34581"
./customerroute gate --listen "127.0.0.1:34570" --gate-address "127.0.0.1:34590"
```There have been several failed attempts to sign in from this account or IP address. Please wait a while and try again later.  
## master 监听 127.0.0.1:34567 
## 127.0.0.1:12345 网页客户端
##  chat1 监听 127.0.0.1:34580 链接master
##  chat2 监听 127.0.0.1:34581 链接master
##  gate  监听 127.0.0.1:34570 链接master
##  gate  监听客户端 127.0.0.1:34590
## open browser and visit url for 4 times
```
http://127.0.0.1:12345/web/ 
http://127.0.0.1:12345/web/ 
http://127.0.0.1:12345/web/ 
http://127.0.0.1:12345/web/     
```
input content and send, the same ChatRoomService node will sync the message each other
