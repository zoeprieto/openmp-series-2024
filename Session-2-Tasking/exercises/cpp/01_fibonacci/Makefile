.PHONY: clean run go debug release

PROG=fibonacci
CC = cc
FLAGS_OPENMP = -fopenmp

release:
	$(CC) -Wall -g $(FLAGS_OPENMP) -O3 ${PROG}.c -o ${PROG}.exe

debug:
	$(CC) -Wall -g $(FLAGS_OPENMP) -O0 ${PROG}.c -o ${PROG}.exe

run go:
	./${PROG}.exe < input

clean:
	rm -f ${PROG}.exe ${PROG}.o *~
