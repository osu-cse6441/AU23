all: serial

CXX = g++
CXXFLAGS = -std=c++11 -O2

serial: cell_auto_ser.C
	$(CXX) $(CXXFLAGS) -o cell_auto_ser $<

clean:
	rm -f cell_auto_ser.o cell_auto_ser
