# suffix rules don't allow pre-requisites to be used and are deprecated for
# this reason.  The right way to do this is to use patterns.  The "%" pattern
# allows any file to be matched.
OBJS = HW4.o Address.o Person.o Employee.o
CXX = g++
INCLUDE = 
LIBS = 
CXXFLAGS = -Wall -g -std=c++11
EXECUTABLE = HW4
COMMANDLINE =

.PHONY : run
run : $(EXECUTABLE)
	./$(EXECUTABLE) $(COMMANDLINE)

cleanmake : clean HW4

.PHONY : $(EXECUTABLE)
$(EXECUTABLE) :  $(OBJS)
	$(CXX) $(XXFLAGS) -o $(EXECUTABLE) $(OBJS) $(INCLUDE) $(LIBS)

%.o : %.c 
	$(CXX) $(CXXFLAGS) -c $@ $(INCLUDE) $(LIBS)

clean :
	rm $(EXECUTABLE) ${OBJS} 
