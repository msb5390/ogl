tutorial03.exe : tutorial03.o ../common/shader.o
	g++ -o tutorial03.exe tutorial03.o ../common/shader.o -lglfw \
	-lglew -framework OpenGL

tutorial03.o : tutorial03.cpp ../common/shader.hpp ../common/shader.cpp
	g++ -c tutorial03.cpp

../common/shader.o : ../common/shader.hpp ../common/shader.cpp
	g++ -c shader.cpp

clean:
	rm tutorial03.o ../common/shader.o