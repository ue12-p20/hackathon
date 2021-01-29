CXX=g++
CXXFLAGS=-Wall -g
RM=rm -f
LIBS=-lncurses

play : nethack.o
	$(CXX) $(CXXFLAGS) $^ $(LIBS) -o $@ 

nethack.o : nethack.cpp

%.o:%.cpp; $(CXX) $(CXXFLAGS) -o $@ -c $<

clean :
	$(RM) all nethack.o ./play

.PHONY: clean
