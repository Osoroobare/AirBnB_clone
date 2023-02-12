# AirBnB Clone - The Console

---

## Description

This project is the first step towards building a full web application of the AirBnB clone. We will use what we build during this project with all other following projects: HTML/CSS templating, database storage, API, front-end integration…

Each task is linked and will help us to:

* put in place a parent class (called BaseModel) to take care of the initialization, serialization and deserialization of your future instances
* create a simple flow of serialization/deserialization: Instance <-> Dictionary <-> JSON string <-> file
* create all classes used for AirBnB (User, State, City, Place…) that inherit from BaseModel
* create the first abstracted storage engine of the project: File storage.
* create all unittests to validate all our classes and storage engine
This console will allow help us to do the following:
* Create a `new object`
* Retrieve an object from a `file, a database etc…`
* Do operations on objects (count, compute stats, etc…)
* Update attributes of an object
* Destroy an object

## Usage

* The console can be run in both interactive and non-interactive mode.
* It prints a prompt **(hbnb)** and waits for the user for input.

### Interactive Mode

```cmd
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```

### Non-Interactive Mode

```cmd
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```

## Commands

Command | Description
--- | ---
`quit` | Exits the program
`EOF` | Exits the program
`create <class>` | Creates an instance of a class
`show <class> <id>` | Prints the string representation of an instance of a class based on class name and id
`destroy <class> <id>` | Deletes instance of a class based on class name and id
`all` | Prints all string representations of all instances
`all <class>` | Prints all string representations of all instances based on class name
`update <class> <id> <attribute name> "<attribute value>"` | Updates an attribute of an instance based on class name and id
`<class>.all()` | Retrieves all instances of a class
`<class>.count()` | Retrieves the number of instances of a class
`<class>.show(<id>)` | Retrieves an instance based on its id
`<class>.destroy(<id>)` | Destroys an instance based on its id

---

## Authors

* **Osoro Obare** - Github: [Osoroobare](https://github.com/Osoroobare) 
* **Ayodeji Ayodeji** - Github: [ayodejix2](https://github.com/ayodejix2) 
