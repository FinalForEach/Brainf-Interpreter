BIN_FOLDER = ../bin
TEST_FOLDER = ../test-programs

INTERPRETER = $(BIN_FOLDER)/interpreter

STD_VER = c++17

all: INTERPRETER



INTERPRETER: BIN_FOLDER
	$(CXX) *.cpp -o $(INTERPRETER) -std=$(STD_VER)
	
BIN_FOLDER:
	mkdir -p $(BIN_FOLDER)
	
	
test-helloworld: INTERPRETER
	$(INTERPRETER) $(TEST_FOLDER)/Hello\ World
	
test-hellocomplex: INTERPRETER
	$(INTERPRETER) $(TEST_FOLDER)/Hello\ World\ Complex
	
test-cat0: INTERPRETER
	$(INTERPRETER) $(TEST_FOLDER)/Cat0
	
test-cellsize: INTERPRETER
	$(INTERPRETER) $(TEST_FOLDER)/Cell\ Size
clean:
	rm -rf $(INTERPRETER)
