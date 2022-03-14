# Welcome to the Jaseci Tutorial

Hi! The First thought come to our mind after knowing that we have to learn a new programming language, Jaseci is, WHY, a new language?
Let's achieve the answer together by learning some facts 

# Jaseci is a computational model and a language in one unit
In simple words, **Jaseci** provides a platform where you can implement the SOTA AI modules without taking the pain of training or hosting them. 


## Starting With Jaseci
1. Getting **Jac** in your local system: 
   1. Pypi Installation : pip install jaseci-core (gets you the latest jac version)
   2. getting from the github :
      1.  git clone https://github.com/Jaseci-Labs/jaseci.git
      2.  cd  **jaseci_core**
      3.   bash install.sh
2. Starting With **jsctl** :
   1. once you fire **jsctl** command in out terminal, jaseci command line shell it activated.
        >
            jsctl
            Starting Jaseci Shell...
            jaseci > 
   2.  type `help`
        >
            jaseci > help

            Documented commands (type help <topic>):
            ========================================
            actions    clear   global  logger  master  sentinel  walker
            alias      config  graph   login   object  stripe
            architype  edit    jac     ls      reset   tool

            Undocumented commands:
            ======================
            exit  help  quit 
            
    1. You'll get all available commands that is available in **Jaseci**
    2. For getting details on command you can type :
        > 
            jaseci > graph --help
            Usage: graph [OPTIONS] COMMAND [ARGS]...

            Group of `graph` commands

            Options:
            --help  Show this message and exit.

            Commands:
            active  Group of `graph active` commands
            create  Create a graph instance and return root node graph object
            delete  Permanently delete graph with given id
            get     Return the content of the graph with mode Valid modes: {default,...
            list    Provide complete list of all graph objects (list of root node...
            node    Group of `graph node` commands
## Coding the Jac File
1. Before jumping into the code let's know about the building blocks of jac programming. Everything in **Jac** is about graph, therefore, **Nodes** and **Edges** are the main constituient of jac programming, now to traverse through graph **Jac** has a superman known as **Walker**. 
   
2. `Hello World` :
    Let's Start with our first Jac program. 
    >  
        walker init {
        std.out("hello world");
        }
    Save the above code in `hello_world.jac` file in the current working directory.
    > 
        jaseci > jac run hello_world.jac
        2022-03-14 16:24:35,847 - INFO - parse_jac: default: Processing Jac code...
        2022-03-14 16:24:35,905 - INFO - register: default: Successfully registered code
        hello world
    
