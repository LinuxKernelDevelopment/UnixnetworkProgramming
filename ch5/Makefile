include Makefile.include

.PHONY: _all tcpservcli clean
_all: tcpservcli

tcpservcli: tcpserv tcpcli

tcpserv: tcpcliserv/tcpserv01.c lib/str_echo.c -lunp
	${CC} -o $@ $^ -lunp
tcpcli: tcpcliserv/tcpcli01.c lib/str_cli.c -lunp
	${CC} -o $@ $^ -lunp

clean:
	${RM} tcpserv tcpcli
