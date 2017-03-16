tutorial04.exe : tutorial04.o ../common/shader.o
	g++ -o tutorial04.exe tutorial04.o ../common/shader.o \
	-lglfw -lglew -framework OpenGL

tutorial04.o : tutorial04.cpp ../common/shader.hpp
	g++ -c tutorial04.cpp

../common/shader.o : ../common/shader.cpp ../common/shader.hpp
	g++ -c ../common/shader.cpp -o ../common/shader.o

clean:
	rm ../common/shader.o tutorial04.o