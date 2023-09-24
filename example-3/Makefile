# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = hello
DEBUG_EXEC    = hello-dbg
TARGET = Kazino-Royal.cpp

all: debug release

debug: $(DEBUG_EXEC)

hello-dbg: $(TARGET)
	g++ $(DEBUG_FLAGS) $(TARGET) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

hello: $(TARGET)
	g++ $(RELEASE_FLAGS) $(TARGET) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)

