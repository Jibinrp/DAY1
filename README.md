DAY1
DIFFERENCE BETWEEN HTTP/1.1-HTTP/2

HTTP/1.1

Ithe usest works on the textual format.
There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.
It uses requests resource Inlining for use getting multiple pages
It compresses data by itself.

HTTP/2

It works on the binary protocol
It allows multiplexing so one TCP connection is required for multiple requests.
It uses PUSH frame by server that collects all multiple pages 
It uses HPACK for data compression.

Objects and its internal representation in Javascript


Object:
In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

Creating Objects in JavaScript:
By object literal!
By creating instance of Object directly (using new keyword)
By object literal:
object={property1:value1,property2:value2...propertyN:valuen}

The syntax of creating object using object literal is given below:


Property and value is separated by colon(:).

Example:

var person={
fname:"xxx",
lname:"yyy",
age:25
};


By creating instance of Object directly (using new keyword):
The syntax of creating object directly is given below:

var objectname= new object();

Here, new keyword is used to create object.

Example:

var emp=new object();
emp.id=101;
emp.name="xxx"
emp.salary=5000;

Accessing JavaScript Objects:
The syntax for accessing the property of an object is:

objectName.property

or

objectName[“property”]

Accessing ‘fname’ from example 1 using dot operator,
person.fname


Accessing ‘name’ form example 2 using [],
emp["name"]






HTTP2 is much faster and more reliable than HTTP1. HTTP1 loads a single request for every TCP connection, while HTTP2 avoids network delay by using multiplexing. HTTP is a network delay sensitive protocol in the sense that if there is less network delay, then the page loads faster.
