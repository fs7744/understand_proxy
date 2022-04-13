# Socket

```
func Socket(domain, typ, proto int) (fd int, err error)
listen()
connect()
accept()
recvmsg()/sendmsg()
close()
```

https://man7.org/linux/man-pages/man2/socket.2.html

## option

SetsockoptInt (in syscall)

- syscall.TCP_NODELAY
- syscall.SO_KEEPALIVE
- syscall.TCP_KEEPINTVL
- syscall.TCP_KEEPIDLE
- syscall.SOL_SOCKET, SO_ZEROCOPY
- unix.SO_RCVBUF
- unix.SO_SNDBUF

server:

- unix.SO_REUSEPORT
- unix.SO_REUSEADDR

liunx vs bsd vs darwin
