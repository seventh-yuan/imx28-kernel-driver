EXEC		= fm24_test
OBJS		= test.o
CROSS 		= arm-fsl-linux-gnueabi-
CC			= $(CROSS)gcc
STRIP		=$(CROSS)strip
CFLAGS 		= -Wall -g -O2


all: clean $(EXEC)

$(EXEC): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $(OBJS)
	$(STRIP) $@

clean:
	rm -rf $(EXEC) *.o