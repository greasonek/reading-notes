# Class 05 Reading Notes

## Building a server *Definitions List*

- **Server** -
  - Anything that can take a request and serve back an answer; A middleman host for the browser where information is stored; 'server' and 'app' are interchangeable in terms of building a route
  - examples: functions, a laptop

- **Node.js** -
  - A JavaScript runtime used to build a server; A tool that makes apps dynamic; Uses asynchronous input and output

- **Modular Code** -
  - Re-useable blocks of code for plug and play; readable, reusable and scalable code

- **HTTP** -
  - Hypertex Transfer Protocol - directive standardization of an action or procedure (a standard way of transferring documents over the internet)

- **Data Structure** -
  - A common way to organize data like an object that can be a container or another form of organization for holding data; An object that can be used for holding data for a person like a customer for example, it would hold information about their name, age, height, weight, etc.
  
- **C.R.U.D.** -
  - C - CREATE - add something (a new record) to a database (post)
  - R - READ - retrieving a record(s) (get)
  - U - UPDATE - update an existing record with new data (put)
  - D - DELTE - delete a record(s) (delete/destroy)

- **MongoDB** -
  - A non-relational database that does not use rows or columns found in traditional databases; holds records on their own but are not linked to one another; all the records held look the same because we assign them a *model* (or schema) but they are not necessarily related

- **SQL** -
  - *Structured Query Language* - A standard language used to create and manipulate a database; best fit for the complex query intensive environment; SQL databases are vertically scalable meaning you can increase the load on a single server

- **Big O** -
  - An explanation of how complex an algorithm is, how much time it takes to complete and how much memory (space) is used
    - measured by O(n) or O(1)
    - O(1) means it takes **constant time** to run an algorithm regardless of the size of the input --> *examples: math operations, accessign an array via the index, returning a value*
      - *real life example: a bookmark - allows a reader to find the last page they were reading efficiently and quickly regardless of the size of the book in one single step <a href="https://www.linkedin.com/pulse/big-o-notation-simple-explanation-examples-pamela-lovett/">Source</a>*
    - O(n) means linear time or the time it takes to run an algorithm increases as the input increases --> *examples: Javascript methods like forEach(), map(), and reduce()*
      - *real life example: reading a book takes linear time, reading one page may take 1 minute so 30 pages would take 30 minutes, 100 pages would take 100 minutes, etc.<a href="https://www.linkedin.com/pulse/big-o-notation-simple-explanation-examples-pamela-lovett/">Source</a>*

## LINKED LIST

- Traversal: the process of moving from one data point to another data point

- example:

**NODE CLASS**

class Node {
  constructor(value, next=null) {
    this.value = value;
    this. next = next;
  }
}

- example:

**LINKED LIST CLASS**

class LinkedList {
  constructor(){
    this.head = null;
  }
  addOne(value) {
    if (!this.head) {
      this.head = new Node (value);
    } else {
    const temp = new Node(value);

    // *PROPERTIES A NODE HAS: VALUE AND NEXT*
    // *DEFAULT VALUE OF NEXT IF NULL IF IT'S NOT GIVEN A VALUE*
    temp.next = this.head;

    //make temp the NEW HEAD
    this.head = temp;

    // *THIS ADDS A NEW NODE TO THE BEGINNING OF THE LINKED LIST*
    // *FUNCTION RUNS, 'TEMP' GOES AWAY AND 'HEAD' PERSISTS, NOW WE HAVE A NEW STARTING POINT*
    }
  }
}

**HOW TO TRAVERSE THROUGH LINKED LIST** (TRAVERSAL)

// travel from head node to the last node and return the last value

traversal() {
  if (!this.head) return 'the list is empty';
  let current = this.head;
  while (current.next){
    // CHECK FOR THE VALUE YOU WANT, IF NO VALUE, KEEP GOING THROUGH LOOP
    // IF THERE IS A VALUE YOU WANT, STOP AND RETURN CURRENT
    current = current.next;
  }
  //AT END OF LINKED LIST WANT TO END WHILE LOOP SO WE DON'T CRASH
  return current;
  // IF NO NODE CONTAINS THE VALUE WE WANT:
  return 'the value does not exist';
}

traversalCheatSheet() {
    let current = this.head;
    while(current) {
      current = current.next;
    }
  }
  altTraveralCheatSheet() {
  let current = this.head;
    if (!current) return
    while(current.next) {
      current = current.next;
    }
    return current;
  }
}

traverseAndPrint(value) {
  let current = this.head;
  while(current) {
    console.log(current.value);
    current = current.next;
  }
}