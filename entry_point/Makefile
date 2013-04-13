
TARGET = entry

CPP_FLAGS =
LD_FLAGS  = 

OBJS = $(patsubst %.cpp, %.o, $(wildcard *.cpp))

%.o: %.cpp
	g++ -std=c++0x -g -c $< -o $@ $(CPP_FLAGS)

all: $(TARGET)

$(TARGET): $(OBJS)
	g++ $(OBJS) $(LD_FLAGS) -o $(TARGET)

clean:
	rm -f $(TARGET) $(OBJS) core* *~
