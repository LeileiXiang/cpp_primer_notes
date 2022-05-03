ifeq ($(OS),Windows_NT)
RM = del
CP = copy
else
RM = rm
CP = cp
endif

objs = test.o

all: test
	./test

test: $(objs)
	g++ -o test $(objs)

.PHONY: clean
clean:
	-$(RM) test test.exe $(objs)
