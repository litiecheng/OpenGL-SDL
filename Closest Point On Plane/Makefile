CC			= g++

TARGET		= ClosestPointOnPlane

$(TARGET):	Main.o Init.o 3DMath.o
	$(CC) -o $(TARGET) Main.o Init.o 3DMath.o `sdl-config --libs` -lGL -lGLU -lm

Main.o:		Main.cpp main.h
	$(CC) -c Main.cpp `sdl-config --cflags`
 nit.o:		Init.cpp main.h
	$(CC) -c Init.cpp `sdl-config --cflags`

3DMath.o:	3DMath.cpp main.h 3DMath.h
	${CC} -c 3DMath.cpp `sdl-config --cflags`

clean:
	rm -f $(TARGET) Main.o Init.o 3DMath.o core
