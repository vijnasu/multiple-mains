# multiple-mains
Passing command line arguments to multiple main programs with and without namespace in C++

Compile:
```
g++ -I./ -c -o main2.o main2.cpp
g++ -I./ main1.o main2.o -o main main.cpp
```

Run:
```
./main 5
```

output:
```
Inside main1's Main without namespace: argv[1]: 5
Inside main2's Main with namespace: argv[1]: 5
```
