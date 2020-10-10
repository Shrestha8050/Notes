# Node.js

    Node.js is an open source, cross-platform, back-end Javascript runtime (server) envirmonent that executes JavaScript code outside a web browser.

_Node.js uses JavaScript on the server_
_Node.js runs single-threaded, non-blocking, asynchronously programming, which is very memory efficient._

Node.js represents a "JavaScript everywhere" paradigm.

### Open Source

    Original source code that is freely available and may be redistributed and modified according to the requirement of the user.

### Cross Platform

    Software that can run on multiple types of computer systems (Windows, Linux, Unix, Mac OS X, etc.)

## Back-End

    Refers to any part of a website or software program that users do not see.

# Why Node.js

**Node.js uses asynchronous programming!** means instead of waiting for unit process to be complete, it handles the all the process and notify/return process result according to the operation( Blocking or Non-Nlocking ) of the process.

- Blocking operation : this operation block further execution untilll that operation finishes.
- Non-Blocking : This operation refers to code that doesnt block execution.
- Asynchronous Programming means a parallel programming in which a unit of work runs separately from the main application thread and notifies the calling thread of its completion, failure or progress.

### How Node.js Works

         Node.js eliminates the waiting and simply continues with the next request.

### How Node.js handles file request

1. Sends the task to the computer's file system.
2. Ready to handle the next request.(Because Using the file system takes time)
3. When the file system has open and read the file, the server returns the content to the client.
