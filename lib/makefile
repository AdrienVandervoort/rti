.SILENT:

CXX = g++
CXXFLAGS = -I/usr/include/mysql -m64
LDFLAGS = -L/usr/lib64/mysql -lmysqlclient -lpthread -lz -lm -lrt -lssl -lcrypto -ldl


tcp.o: tcp.c tcp.h
	echo Creation de tcp.o
	$(CXX) $(CXXFLAGS) -c tcp.c -o tcp.o

ovesp.o: ovesp.h ovesp.cpp
	echo Creation de ovesp.o
	$(CXX) $(CXXFLAGS) -c ovesp.cpp -o ovesp.o

clean:
	rm -f ./*.o
	rm -f testServer
	rm -f testClient
