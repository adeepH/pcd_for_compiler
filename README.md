## CSPC41 Compiler Design Project Assignment

# Compiler Design Project: Simulation of front-end phase of C Compiler involving switch-case construct.

Using lex/yacc implement a parser for managing the `switch` statement in a simplified version. 

* The variable used in the switch is one integer variable in a predefined set of two variables `x`, `y`.

* The switch instruction has the following syntax
    ```
    switch(var) {
        case 0: 
            z=cost0;
            break;

        ...

        case N: 
            z=costN;
            break;

        default: 
            z=costD;
            break;
    }
    ```

* The instruction contains only the assignment of a constant value to the variable `z`.

* At the end print the value of the variable `z`.

## Steps

1. Run the `exe.sh` file:

    ```>>> ./exe.h ```
    
    This line of code will generate the following files:
    
    * `lex.yy.c`
    * `switch.tab.c`
    * `switch.tab.h`
    * `switch`
1. Give permissions to the `exe.sh` file if you get the message `exe.sh permission denied`:
    
    ```>>> chmod +x ./exe.sh ```
3. Run the parser and give it as input one of the files in the `tests` folder:

    ```>>> ./switch < tests/switch_ok1.c```

4. For `tests/switch_ok1.c`, The output should be:

    ```z=209```

Contributors
* CSE18U001 - Adeep Hande
* CSE18U013 - Karthik Puranik
* CSE18U015 - Konthala Yasaswini
* CSE18U017 - Akhil Gupta