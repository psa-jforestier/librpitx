all: testrpitx sendook

CFLAGS	= -Wall -g -O3 -Wno-unused-variable 
LDFLAGS	= -lm -lrt -lpthread 
CCP = g++ 
CC = gcc 


testrpitx: testrpitx.cpp ../src/librpitx.h ../src/librpitx.a
	
	$(CCP) $(CFLAGS) -o testrpitx testrpitx.cpp ../src/librpitx.a $(LDFLAGS)

sendook: sendook.cpp ../src/librpitx.h ../src/librpitx.a
	$(CCP) $(CFLAGS) -o sendook sendook.cpp ../src/librpitx.a $(LDFLAGS)

clean:
	
	rm -f  testrpitx sendook
