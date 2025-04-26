# cs6200-project-1--multithreading-solved
**TO GET THIS SOLUTION VISIT:** [CS6200 Project 1- Multithreading Solved](https://www.ankitcodinghub.com/product/cs6200-multithreading-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;126802&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6200 Project 1- Multithreading Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Foreword

In this project, you will design and implement a multi-threaded server that serves static files based on the GetFile protocol, which is a simple HTTP-like protocol. Alongside the server, you will also create a multi-threaded client that acts as a load generator for the server. Both the server and client will be written in C and be based on a sound, scalable design.

Setup

Please follow the instructions given in the environment repository for setting up your development/test environment. You can clone the code in this repository with the command

console $ git clone https://github.gatech.edu/gios-spr-23/pr1.git

Submission Instructions

We use an auto-grading system based upon Gradescope. You can find Gradescope from Canvas, and that will make the submission engine available to you. You will need to manually upload your code to Gradescope, where it will be executed in its own environment (a Docker container) and the results will be gathered up and returned to you.

Feedback from Gradescope

Note that there is a strict limit to the amount of feedback that we can return to you. Thus:

We do not return feedback for tests that pass

We truncate any feedback past the limit (approximately 10KB)

We do not return detailed feedback for tests that run after the 10KB limit is reached.

We strongly encourage you to think about testing your own code. Test driven development is a standard technique for software, including systems software. The auto-grader is a grader and not a test suite.

Note: your project readme file (10% of your grade for Project 1) is submitted on Canvas in PDF format.

We do not use the “activate” feature

README

Warm-up: Sockets

In this project, your client and server will communicate via sockets. To help you familiarize yourself with Câ€™s standard socket API, you will complete a few warm-up exercises

Echo Client-Server

Most socket tutorials start with a client-server pair where the server simply echoes (that is, repeats back) the message that the client sends. Sometimes referred to as the EchoClient and the EchoServer. In the first part of this assignment, you will turn in a pair of programs that perform these roles.

It is important that the only output (either to stdout or stderr) be the response from the server. Any missing or additional output causes the test to fail.

Your programs should support both IPv4 and IPv6. We have tests in subsequent parts to test support for IPv4 and IPv6.

Once you have completed your programs inside the echo directory, you upload it to Gradescope (which you can find from Canvas).

Once submitted, Gradescope will test your echoclient.c code with its own reference implementation of echoserver.c and your echoserver.c code with its own reference implementation of echoclient.c. It will then return some feedback to help you refine your code if it does not meet requirements.

Transferring a File

In this part of the assignment, you will implement code to transfer files on a server to clients.

The basic mechanism is simple: when the client connects to the server, the server opens a pre-defined file (from the command line arguments), reads the contents from the file and writes them to the client via the socket (connection). When the server is done sending the file contents, the server closes the connection.

/ Preparing message / â€¦

/Sending message / sent = send(socket, buffer, length, 0); assert( sent == length); //WRONG! “`

In fact, it is this strategy that you should employ as the second part of the warm-up. You are to create a client, which simply connects to a server-no message need be sent– and saves the received data to a file on disk.

Beware of file permissions. Make sure to give yourself read and write access, e.g. S_IRUSR | S_IWUSR as the last parameter to open.

server that simply begins transferring data from a file over the network once it establishes a connection and closes the socket when finished.

Your server should not stop after a single transfer, but should continue accepting and transferring files to other clients. Your client should terminate after receiving the full contents. Unlike a normal web server (which leaves the socket open until the client closes it) your server should close the socket so the client knows when the full contents of the file have been transmitted. Note that the length of the file being sent is otherwise not known to the client; adding it to your client and server means it will not pass the grader because it does not implement the same protocol.

Part 1: Implementing the Getfile Protocol

Getfile is a simple (HTTP-like) protocol used to transfer a file from one computer to another that we made up for this project. A typical successful transfer is illustrated below.

The general form of a request is

&lt;scheme&gt; &lt;method&gt; &lt;path&gt; Note:

The scheme is always GETFILE.

The method is always GET.

The path must always start with a â€˜/â€™.

The general form of a response is

&lt;scheme&gt; &lt;status&gt; &lt;length&gt; &lt;content&gt; Note:

The scheme is always GETFILE.

The status must be in the set {â€˜OKâ€™, â€˜FILE_NOT_FOUNDâ€™, â€˜ERRORâ€™, ‘INVALID’}.

FILE_NOT_FOUND is the appropriate response whenever the client has made an error in his request. ERROR is reserved for when the server is responsible for something bad happening.

When the status is OK, the length should be a number expressed in ASCII (what sprintf will give you). The length parameter should be omitted for statuses of FILE_NOT_FOUND or ERROR.

The character ‘ ‘ is a single byte, which when used in a C literal string is translated by the compiler to be a carriage return.

The character ‘ ‘ is a single byte, which when used in a C literal string is translated by the compiler to be a newline character.

‘ ‘.

The space between the and the and the space between the and the are required. There should not be a space betwen the and ‘ ‘. There should not be a space between and ‘ ‘.

Note the strings are not terminated with a null character. The buffers that you receive are not C strings. Just like HTTP, this is a language neutral format. Do not assume that anything you receive is null (”) terminated. You should avoid using string functions unless you have ensured that the data has been null-terminated.

Instructions

For Part 1 of the assignment you will implement a Getfile client library and a Getfile server library. The API and the descriptions of the individual functions can be found in the gfclient.h and gfserver.h header files. Your task is to implement these interfaces in the gfclient.c and gfserver.c files respectively. To help illustrate how the API is intended to be used and to help you test your code we have provided the other files necessary to build a simple Getfile server and workload generating client inside of the gflib directory. It contains the files

Makefile – (do not modify) used for compiling the project components content.[ch] – (do not modify) a library that abstracts away the task of fetching content from disk.

content.txt – (modify to help test) a data file for the content library gfclient.c – (modify and submit) implementation of the gfclient interface.

gfclient.h – (do not modify) header file for the gfclient library gfclient-student.h – (modify and submit) header file for students to modify – submitted for client only gfclient_download.c – (modify to help test) the main file for the client workload generator. Illustrates use of gfclient library. gfserver.c – (modify and submit) implementation of the gfserver interface.

gfserver.h – (do not modify) header file for the gfserver library.

gfserver-student.h – (modify and submit) header file for students to modify – submitted for server only gfserver_main.c (modify to help test) the main file for the Getfile server. Illustrates the use of the gfserver library. gf-student.h (modify and submit) header file for students to modify – submitted for both client and server handler.o – contains an implementation of the handler callback that is registered with the gfserver library. workload.[ch] – (do not modify) a library used by workload generator

workload.txt – (modify to help test) a data file indicating what paths should be requested and where the results should be stored.

gfclient

The client-side interface documented in gfclient.h is inspired by libcurlâ€™s â€œeasyâ€ interface. To help illustrate how the API is intended to be used and to help you test your code, we have provided the file gfclient_download.c. For those not familiar with function pointers in C and callbacks, the interface can be confusing. The key idea is that before the user tells the gfclient library to perform a request, user should register one function to be called on the header (gfc_set_headerfunc) and register one function to be called for every â€œchunkâ€ of the body

(gfc_set_writefunc). That is, one call to the latter function will be made for every recv() call made by the gfclient library. (It so happens that none of the test code actually will use the header function, but please implement your library to support it anyway.)

Note that the gfcrequest_t is used as an opaque pointer, meaning that it should be defined within the gfclient.c file and no user code (e.g.

gfclient_download.c) should ever do anything with the object besides pass it to functions in the gfclient library.

gfserver

The server side interface documented in gfserver.h is inspired by pythonâ€™s built-in httpserver. The existing code in the file gfserver_main.c illustrates this usage. Again, for those not familiar with function pointers in C and callbacks, the interface can be confusing. The key idea is before starting up the server, the user registers a handler callback with gfserver library which controls how the request will be handled. The handler callback should not contain any of the socket-level code. Instead, it should use the gfs_sendheader, gfs_send, and potentially the gfs_abort functions provided by the gfserver library. Naturally, the gfserver library needs to know which request the handler is working on. All of this information is captured in the opaque pointer passed into the handler, which the handler must then pass back to the gfserver library when making these calls.

Submission

You should submit your code via Gradescope.

Part 2: Implementing a Multithreaded Getfile Server

Note: For both the client and the server, your code should follow a boss-worker thread pattern. This will be graded. Also keep in mind this is a multi-threading exercise. You are NOT supposed to use fork() to spawn child processes, but instead you should be using the pthreads library to create/manage threads. You will have points removed if you don’t follow this instruction.

Similarly on the client side, the Getfile workload generator can only download a single file at a time. In general for clients, when server latencies are large, this is a major disadvantage. You will make your client multithreaded by modifying gfclient_download.c. This will also make testing your getfile server easier.

In the client, a pool of worker threads should be initialized based on number of client worker threads specified with a command line argument.

Once the worker threads have been started, the boss should enqueue the specified number of requests (from the command line argument) to them. They should continue to run. Once the boss confirms all requests have been completed, it should terminate the worker threads and exit. We will be looking for your code to use a work queue (from steque.[ch]), at least one mutex (pthread_mutex_t), and at least one condition variable (pthread_cond_t) to coordinate these activities. Gradescope will confirm that your implementation meets these requirements.

Makefile – (do not modify) used for compiling the project components content.[ch] – (do not modify) a library that abstracts away the task of fetching content from disk.

content.txt – (modify to help test) a data file for the content library gfclient.o – (do not modify) implementation of the gfclient interface.

gfclient.h – (do not modify) header file for the gfclient library

gfclient-student.h – (modify and submit) header file for students to modify – submitted for client only gfclient_download.c – (modify and submit) the main file for the client workload generator. Illustrates use of gfclient library.

gfserver.o – (do not modify) implementation of the gfserver interface.

gfserver.h – (do not modify) header file for the gfserver library.

gfserver-student.h – (modify and submit) header file for students to modify – submitted for server only gfserver_main.c (modify and submit) the main file for the Getfile server. Illustrates the use of the gfserver library.

gf-student.h (modify and submit) header file for students to modify – submitted for both client and server handler.c – (modify and submit) contains an implementation of the handler callback that is registered with the gfserver library.

steque.[ch] – (do not modify) a library you must use for implementing your boss/worker queue.

workload.[ch] – (do not modify) a library used by workload generator workload.txt – (modify to help test) a data file indicating what paths should be requested and where the results should be stored.

Grading

Your code should be submitted via Gradescope.

Readme

Throughout your development you should be keeping notes about what you are doing for your development. We encourage you to submit your readme file as your project develops, so that it can serve as a log of your work.

To obtain all possible points, we want you to demonstrate your understanding of what you have done. We are not looking for a diary, we are looking for a clear explanation of what you did and why you did it. This is your grader’s opportunity to award you points for understanding the project, even if you struggle with the implementation, as these are manually graded.

You should upload your README file via Canvas (Project 1 README).

NOTE: This is your opportunity to clearly document your reference materials.

Finally, we encourage you to make concrete suggestions on how you would improve this project. This is not required for the project, but is an opportunity for you to earn extra credit points. This could also include sample code, suggested tests (we really like examples!), ways to improve the documentation, etc.

References

Sample Source Code

Server and Client Example Code – note the link referenced from the readme does not work, but the sample code is valid. Another Tutorial with Source Code for server and client

General References

POSIX Threads (PThreads)

Linux Sockets Tutorial

Practical TCP/IP Sockets in C

Guide to Network Programming

Helpful Hints

High-level code design of multi-threaded GetFile server and client

Return code (exit status) 11 of client or server means it received a SIGSEGV (segmentation fault). You can get a comprehensive list of signals with kill -l.

In the warm-up part, the server should be running forever. It should not terminate after serving one request. Use the class VM to test and debug your code. The autograder is not a test harness.

Rubric

Warm-up (20 points)

Echo Client-Server (10 points) Transfer (10 points)

Your submission should compile and build without any errors on gradescope.

For transfer: Your client should successfully save the file sent from the sever on the disk and the server should accurately send the file to the client. File size and contents on the client should match the file size and contents on the server side.

Part 1: Getfile Libraries (30 points)

Client (15 points)

Server(15 points)

In addition to the above tests , we also run some sanity tests to ensure your submission compiles &amp; builds without any errors on gradescope and proper initialization &amp; cleanup is performed (eg: no memory leaks and no invalid memory accesses).

Part 2: Multithreading (40 points)

Client (20 points)

Server(20 points)

In addition to the sanity tests discussed in part 1, our tests will validate if your submission supports multiple file downloads of varying file sizes concurrently. Your implementation employs boss worker model to distribute work and uses appropriate synchronization mechanisms to protect shared data.

README (10 points + 5 point extra credit opportunity)

Clearly demonstrates your understanding of what you did and why – we want to see your design and your explanation of the choices that you made and why you made those choices. (5 points)

A description of the flow of control for your code; we strongly suggest that you use graphics here, but a thorough textual explanation is sufficient. (2 points)

A brief explanation of how you tested your code. (2 points)

References any external materials that you consulted during your development process (1 point)

Suggestions on how you would improve the documentation, sample code, testing, or other aspects of the project (up to 5 points extra credit available for noteworthy suggestions here, e.g., actual descriptions of how you would change things, sample code, code for tests, etc.) We do not give extra credit for simply reporting an issue – we’re looking for actionable suggestions on how to improve things.

Ideal README – the ideal README file is one that you could have picked up at the start of the project and used it to guide your development. It would explain the choices you considered and why you chose specific approaches to the problem. It won’t complain about the code, the process, how little you know about C, or other things unrelated to the project. It won’t discuss the code; it will discuss the techniques and algorithms.

Questions
