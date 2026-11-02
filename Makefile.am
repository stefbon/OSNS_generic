bin_PROGRAMS =
sbin_PROGRAMS =

CC = gcc
RM = rm -f

extra_CFLAGS    = -fexceptions -fstack-clash-protection -Wall -Wextra -Wconversion -Wformat-security 
debug_CFLAGS    = -ggdb -Og
TARGET          =

osns_generic_CFLAGS = $(CFLAGS) $(extra_CFLAGS) $(debug_CFLAGS) -D_FILE_OFFSET_BITS=64 -lz -lpthread -fPIC -lm -lsystemd -losns -I /usr/include/osns-1 -Wall -Wno-unused-but-set-variable -Wno-uninitialized -Wno-unused-variable -Wno-unused-label -Wno-unused-function
osns_generic_LDFLAGS = -L/usr/lib64/libosns.so
osns_generic_SOURCES = main.c

sbin_PROGRAMS += osns_generic

.PHONY: clean

