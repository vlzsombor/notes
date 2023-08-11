* get the strings of an executable
    ```
    strings a.out 
    ```
* get symbols
    ```
    readelf --symbols a.out
    objectdum -t a.out
    ```

* symbols involved
    ```
    objectdum -s a.out
    ```
* disassembly
    ```
    objectdum -d a.out
    ```

[s](https://youtu.be/bWMIpHVRFUo?t=197)


c code segments:

(higher memory segment)

Environment: Command line arguments, environment variables

Stack: storing stack frame, function information (local varaiables) Stack frame is popped from stack when function returns

Heap: Dynamic memory allocation that happens during program execution

Heap memory must be managed by the program statements

malloc realloc calloc free

Data: Un/initialized data
Global & static variables that are initialized
Lifetime of varibale throught the execution of the program
Variables can be changed


Text\Code: Compiled Program instruction. Lower to not be overwritten by heap or stack. It might be shared by multiple processes. 
(lower memory segment)

[s](https://www.youtube.com/watch?v=m1UzSfgjA4Y&ab_channel=VijayVishwakarma)