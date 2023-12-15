# 这是一个注释
CC = gcc

test_sqlist: sqlist_main.o sqlist.o status.o
	$(CC) -o test_sqlist $^

sqlist_main.o: Sqlist_main.c SqList.h 
	$(CC) -c Sqlist_main.c -o sqlist_main.o
sqlist.o : SqList.c SqList.h ../../Status/Status.h
	$(CC) -c SqList.c -o sqlist.o
status.o: ../../Status/Status.c ../../Status/Status.h
	$(CC) -c ../../Status/Status.c -o status.o
clean:
	rm *.o test_sqlist