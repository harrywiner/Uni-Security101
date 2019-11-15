# Memory Corruption

## Uninitialized read

* C does not clean memory on creation of a variable, only on initialization
``` C
    int main()
    {
        int a;
        printf("a: %d\n", a); 

        return 0;
    }
```
* This prints out whatever was stored in the memory reference for `a`





## Format String Errors

* a **format string** is a string in a print statement with the %s before it 
``` C
    printf("Hello"); // Unformatted string

    printf("%s", "Hello"); // Formatted string
```

* a **variadic function** is a function that can take a *variable* number of inputs
``` C
    int main(int aargc, char ** aargv)
    {
        int i = 0xAABBCCDD;
        char secret[] = "SECRET";

        if(aargc > 1)
            printf(aargv[1]);
        return 0;
    }
```

A simple main function that prints out the input of main

```
    input:
    ./test.o %x%x%x%x%x
```

* On a 32 bit system this prints out the value of `i`\
    -> because the computer is looking for a hex value from `%x`


## Integer Operation Errors
* Converting between signed and unsigned integers can lead to errors

### Overflow 
* When an integer is increased or decreased across its limit\
-> Can be unsigned or signed
* This example prints -2147483648 (INT_MIN)
``` C
    i = INT_MAX;
    i++;
    printf("i = %d\n", i); 
```
* A good line of code to check for overflow is:
``` C
    a > UINT_MAX - b
```


## Truncation
* When an integer is converted to a smaller type and the value is out of range\
-> Lower order bits are preserved and higher order bits are lost
``` C
    long d = LONG_MAX;
    printf("d = %d", d); // prolly prints INT_MIN idk tho
```

