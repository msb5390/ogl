tutorial02.exe : tutorial02.o ../common/shader.o
	g++ -o tutorial02.exe tutorial02.o ../common/shader.o \
	-lglew -lglfw -framework OpenGL

tutorial02.o : tutorial02.cpp ../common/shader.hpp
	g++ -c tutorial02.cpp

../common/shader.o : ../common/shader.cpp ../common/shader.hpp
	g++ -c ../common/shader.cpp -o ../common/shader.o

clean:
	rm tutorial02.o ../common/shader.o