CFLAGS := -Wall -O0 -g
CFLAGS += $(shell pkg-config --cflags libdrm gbm)
LDFLAGS := -lcairo
LDFLAGS += $(shell pkg-config --libs libdrm gbm)

kms-pageflip: kms-pageflip.c
	gcc -o $@ $< $(CFLAGS) $(LDFLAGS)

clean:
	rm -f kms-pageflip

.PHONY: clean
