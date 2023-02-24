
objects = addition.o subtraction.o multiplication.o division.o main.o

calculator: $(objects) 
	cc -o calculator $(objects) 

$(objects): %.o:%.c operations.h
	cc -c $< -o $@
# main.o: main.c operations.h
# 	cc -c main.c -o main.o

clean:
	rm -f calculator $(objects)
.PHONY: clean

