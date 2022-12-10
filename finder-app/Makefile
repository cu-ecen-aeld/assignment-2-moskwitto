# Set the compiler and target architecture
CC = aarch64-linux-gnu-gcc
TARGET = arm64

# Set the target binary name
TARGET_BIN = writer

# Set the source file
SRC = writer.c

# Set the CFLAGS for the target architecture
CFLAGS = -march=$(TARGET)

# Build the target binary
$(TARGET_BIN): $(SRC)
    $(CC) $(CFLAGS) -o $(TARGET_BIN) $(SRC)
# Compile the object files
%.o: %.c
    $(CC) $(CFLAGS) -c $<

# Clean up the build directory
clean:
    rm -f $(TARGET) $(OBJECTS)
