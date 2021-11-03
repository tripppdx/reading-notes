### Readings: Socket.io

#### 1. What is the benefit of transforming data into packets?

Transforming data into packets allows more computers to more efficiently share the same bandwidth (one does not have to wait until another is finished with a long message before communictaion). Packets can also adapt to changing network conditions and take the most efficient path to their destination.

https://www.cloudflare.com/learning/network-layer/what-is-a-packet/

#### 2. UDP is often refereed to as a connectionless protocol. Why is this?

With UDP, a connection does not need to established between the source and destination before data is transmitted. Data is sent as soon as it's ready and assumes the endpoint will receive it. It expects expects the application to put the data back together instead of the protocol.

https://www.sciencedirect.com/topics/computer-science/connectionless-protocol

#### 3. Can a socket server application have multiple socket connections?

Yes.

#### 4. Can a socket connection application be connected to multiple socket servers?

Yes.

#### 5. Can an application be both a socket server and a socket connection?

Yes.

#### Document the following Vocabulary Terms

##### Observer Pattern

The observer pattern is a software design pattern in which an subject (server), notifies observers (clients) automatically of any state changes.

https://en.wikipedia.org/wiki/Observer_pattern

##### Listener

A client that 'listens' for events from a server and handles them.

https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events

##### Event Handler

A callback function that is triggered by an event.

https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events

##### Event Driven Programming

"Event driven" is a programming paradigm that consists of user actions/interactions that trigger the next flow of events.

https://hasura.io/event-driven-programming/

##### Event Loop

The event loop JavaScript to perform non-blocking I/O operations — despite being single-threaded

https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/

##### Event Queue

Where asynchronous code gets queued and waits for the execution.

https://medium.com/@Rahulx1/understanding-event-loop-call-stack-event-job-queue-in-javascript-63dcd2c71ecd

##### Call Stack

Where all your JavaScript command gets pushed and executed.

https://medium.com/@Rahulx1/understanding-event-loop-call-stack-event-job-queue-in-javascript-63dcd2c71ecd

##### Emit/Raise/Trigger

An message emission can raise or trigger an event in event driven programming.

https://stackoverflow.com/questions/2490825/how-to-trigger-event-in-javascript

##### Subscribe

Listening to a particular socket.

https://socket.io/docs/v3/rooms/

##### database

A database is an organized collection of structured information, or data, typically stored electronically in a computer system.

https://www.oracle.com/database/what-is-database/
