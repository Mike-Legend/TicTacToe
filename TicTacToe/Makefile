.POSIX:

C++ := /usr/bin/c++
CFLAGS := -c -g
DOS2UNIX := /usr/bin/dos2unix

SRC = main.cpp
OBJ = ${SRC:.cpp=.o}
NAME = TicTacToe

all: ${NAME}

${NAME}: ${OBJ}
	${C++} -o $@ ${OBJ}

.cpp.o:
	${DOS2UNIX} $<
	${C++} ${CFLAGS} -o $@ $<

clean:
	rm -f ${OBJ} ${NAME}
