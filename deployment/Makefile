
# function to check required arguments
check_defined = \
	$(strip $(foreach 1,$1, \
		$(call __check_defined,$1)))
__check_defined = \
	$(if $(value $1),, \
		$(error Undefined $1))

all:
	echo "const char SECRETKEY[16] = {0x46,0x92,0xbf,0x9a,0x9a,0x98,0x80,0x3c,0xe1,0xcf,0xcd,0x0f,0x29,0x57,0x7e,0x0d};" > global_secrets.h

clean:
	rm -f global_secrets.h
