objects= daytimetcpsrv daytimetcpcli_ipv6 daytimetcpcli
all: $(objects)

clean:
	$(RM) $(objects)
$(objects): %: %.c
	$(CC) $< -lunp -o $@
