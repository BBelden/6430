all:	libpp.a ppexec

ppexec:	ppexec.cpp 
	g++ -std=c++11 -o ppexec ppexec.cpp -lpp -L.
	cc -o p4_tester p4_tester.c -lpp -L.

libpp.a:	mpi.c
	cc -c -o mpi.o mpi.c
	ar rvf libpp.a mpi.o

clean:
	rm -f ppexec libpp.a *.o p4_tester
