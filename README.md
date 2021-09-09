# interview_prep
### Python
- basic data types
- why set vs dict
- mutable and immutable
- pass list/str to func and change it
- memory allocation how?
- call super class method
- object type in python
- decorator / generator
- monkey patching (with db function that takes a day to complete)
- unit testing
- multithreading with cores?
- how multithreading
- why with keyword
- what is iterators --> why to use them?
- why sets are there in python
- tuple, list as key in dict?
- cpu intensive tasks ? threading or processing?

### NodeJS
- What is event loop and how async works?
- External library for async?

### Javascript
- '==' and '==='
- Async lib
- how event loop
- set in es6
- how async works?
- mulltithreading in js
- how promises work in js
- how to handle two request response using then?
- let vs var
- [Shallow and Deep copy](https://www.javascripttutorial.net/object/3-ways-to-copy-objects-in-javascript/)

#### why to use typescript?
- Makes code easier to read and understand
- Avoid painful bugs of type checking
- Provides OOP features like interface, classes, inheritance and generics

### Web
- HTTP status codes
- REST API and security

### AWS
- EC2 [QA](https://www.wisdomjobs.com/e-university/aws-ec2-interview-questions.html)
- [QA 2](https://career.guru99.com/top-15-aws-interview-questions/)
- Security groups in EC2
- AMI
- S3 security restrictions ?

### db
- Redis ? why it is used?
#### Mongodb
- Indexing in mongodb
- Horizontally scalable (can store multiple collections on different nodes - Sharding)
- No fixed schema (Unstructured data)
- Rapid Development (does not require schema to be prepared up front)
- High availability (Replication)
- Speed (High performace for simple queries)

##### Not so Good For:
- Highly transactional systems or where the data model is designed up front.
- Tightly coupled systems



```
function func1(name) {
  return new Promise((res, rej) => {
    setTimeout(() => res(name), 300);
  });
}

let x = new Promise((res, rej) => {
    setTimeout(() => res('my promise'), 1000);
  });

/*
x.then(res => {
  console.log(res);
  return func1('one');
 }
)
.then(r => func1('two'))
.then(e => console.log(e));

y = Promise.all([x, func1('all')]);
y.then(r => console.log(r));*/

async function test_async() {

  let y = await x;
  console.log(y);

  let z = await func1('mehul');
  console.log(z);
}

test_async()
```
