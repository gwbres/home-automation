MSPDIR ?= /usr/bin
CC = $(MSPDIR)/msp430-gcc

MCU = msp430g2553

CFLAGS = -0s -Wall -g -mmcu=$(MCU)

OBJ = main
SRCS = xbee.c

RM = rm -rf

$(OBJ): $(OBJ).c
	$(CC) $(CFLAGS) $(OBJ).c -o $(OBJ).elf $(SRCS)

clean:
	$(RM) $(OBJ).elf
