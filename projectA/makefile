main:main.c libbcal.a
	gcc main.c -o main -lcal -Iinclude -Llib
libbcal.a:lib/sub.o lib/add.o
	ar rcs libcal.a  lib/sub.o lib/add.o
lib/sub.o:src/sub.c
	gcc -c src/sub.c -o lib/sub.o -Iinclude
lib/add.o:src/add.c
	gcc -c src/add.c -o lib/add.o -Iinclude
clean:
	rm lib/*.o
	rm lib/main
