.PHONY: clean exec
OBJECTS = client.o client_impl.o ../commun/message.o
CFLAGS =  -p -g

IFLAGS = -I ../commun/


client : $(OBJECTS)
	gcc $(CFLAGS) -o client $(OBJECTS)
client.o : client.c 
	gcc $(CFLAGS) -c client.c $(IFLAGS)
client_impl.o : client_impl.c
	gcc $(CFLAGS) -c client_impl.c $(IFLAGS)


clean :
	rm -f client $(OBJECTS) gmon.out

exec : 
	./client
