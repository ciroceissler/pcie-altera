#
TARGET = PCIE_FUNDAMENTAL

#
CFLAGS = -g -Wall
LDFLAGS = -g -Wall -ldl
CC = g++

build: $(TARGET)

$(TARGET): $(TARGET).o PCIE.o
	$(CC) $^ $(LDFLAGS) -o $@

%.o : %.c
	$(CC) $(CFLAGS) -c $< -o $@

%.o : %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

.PHONY: clean
clean:
	rm -f $(TARGET) *.a *.o *~

