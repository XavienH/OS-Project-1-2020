CFLAG = -DDEBUG -Wall -std=c99

main: main.o process.o
	gcc $(CFLAG) main.o process.o -o main
main.o: main.c Makefile
	gcc $(CFLAG) main.c -c
process.o: process.c process.h Makefile
	gcc $(CFLAG) process.c -c
clean:
	rm -rf *o
run:
	sudo ./main
