all:
	cython -3 -o helloworld.c helloworld.pyx
	gcc -g -O2 -fpic -c helloworld.c -o helloworld.o `python-config --cflags`
	gcc -g -O2 -shared -o helloworld.so helloworld.o `python-config --libs`

clean:
	rm -f helloworld.c helloworld.o helloworld.so


