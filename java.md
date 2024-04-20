- int cannot be converted to boolean, and vice versa
```java
int i = (int)true; //error
while (1); //error
for (;;); 
```

- no unsigned variants, except char(u16)
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
