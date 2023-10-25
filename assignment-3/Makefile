# Modify as needed to work on OSC systems.

CXX = g++
CXXFLAGS = -std=c++11
CUDA = nvcc
CUDAFLAGS = -std=c++11 -O2 -Xcompiler "$(CXXFLAGS)"
GENCODE=--generate-code arch=compute_80,code=sm_80

TARGET = cell_auto_gpu

all: $(TARGET)

cell_auto_gpu: cell_auto_gpu.cu
	$(CUDA) $(CUDAFLAGS) $(GENCODE) -o $@ $<

clean:
	rm $(TARGET) 