# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino-Royal
DEBUG_EXEC    = Kazino-Royal-dbg
name         = Kazino-Royal.cpp

all: debug release

debug: $(DEBUG_EXEC)

Kazino-Royal-dbg: $(name)
	g++ $(DEBUG_FLAGS) $(name) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

Kazino-Royal: $(SRC)
	g++ $(RELEASE_FLAGS) $(name) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)

