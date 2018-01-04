CC = g++
#Using -Ofast instead of -O3 might result in faster code, but is supported only by newer GCC versions
CFLAGS = -lm -pthread -Ofast -march=native -Wall -fexceptions -funroll-loops -Wno-unused-result -Wwrite-strings

all: wordembedding
wordebedding : wordebedding.cpp
	$(CC) wordebedding.cpp -o wordebedding $(CFLAGS)
	chmod +x *.sh

clean:
	rm -rf wordembedding
