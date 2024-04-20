- int cannot be converted to boolean, and vice versa
```java
int i = (int)true; //error
while (1); //error
for (;;); 
```

- no typedef
```c
typedef char u16; //error
```

- no unsigned variants, except char
```java
byte b = 128; //error
char c = -1; //error
```

- initialize an array
```java
int a[3]; //error
int len = 3;
int a[] = new int[len];
```

- no goto
```java
loop:
for(;;)
  for(;;)
    break loop;
```

- string
```java
char str[] = "test"; //error
String str = "test";
char c = str[0]; //error
```

- for loop
```java
int a[] = {1,2,3};
for (int i : a)
    System.out.println(i);
```
