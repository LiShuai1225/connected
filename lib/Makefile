SRCS := $(shell ls *.c)
OBJS := $(SRCS:%.c=%.o)

CFLAGS  += -I$(TOPDIR)/lib/include

LIBOBJ=libx.a

all: $(LIBOBJ)

clean:
	@rm -rf $(LIBOBJ)
	@rm -rf $(OBJS)

$(LIBOBJ): $(OBJS)
	$(AR) rcs $@ $^
