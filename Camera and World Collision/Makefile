CC			= g++

TARGET		= CameraWorldCollision

$(TARGET):	Main.o Init.o 3DMath.o Camera.o
	$(CC) -o $(TARGET) Main.o Init.o 3DMath.o Camera.o `sdl-config --libs` -lGL -lGLU -lm

Main.o:		Main.cpp main.h
	$(CC) -c Main.cpp `sd config --cflags`

Init.o:		Init.cpp main.h
	$(CC) -c Init.cpp `sdl-config --cflags`

3DMath.o:	3DMath.cpp main.h 3DMath.h
	${CC} -c 3DMath.cpp `sdl-config --cflags`

Camera.o:	Camera.cpp main.h Camera.h
	${CC} -c Camera.cpp `sdl-config --cflags`

clean:
	rm -f $(TARGET) Main.o Init.o 3DMath.o Camera.o core 
