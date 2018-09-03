CC = gcc
OBJS = MySocket.o MyClient.o
TARGET = MyClient


#SUFFIXES는 알아서 .c .o의 규칙을 적용시켜줌 gcc -c -o MySocket.o MySocket.c를 해줌
.SUFFIXES: .c .o

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) -o $@ $(OBJS)

clean:
	rm -f $(OBJS) $(TARGET)

MySocket.o: MySocket.c MySocket.h
MyClient.o: MyClient.c MySocket.h

