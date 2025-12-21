This project implements the Producer-Consumer problem: 
 1. Python threading
 2. Semaphores for synchronization
 3. XML for data exchange
 4. Socket programming

The code: 
1. Producer generates random student data
2. Consumer processes XML data
3. Thread-safe buffer of size 10
4. Socket communication between producer and consumer

The producer-consumer is implemented as follows: The producer generates random student information and stores it in an ITStudent class. The variables of the ITStudent class are generated randomly. The variables include: StudentID (8 digit) , Student name, Programme, list of Courses and the associated mark for each course. It then wraps the student information into XML format and saves it to files. The XML files are placed in a directory shared with the buffer and the corresponding integer is inserted into the buffer/queue. 

The consumer reads the content of the XML files shared with the buffer and removes the corresponding integer from the buffer/queue. It then unwraps the XML files and gathers the student information into an ITStudent class. The consumer clears or deletes the XML file an calculates the average mark of the student's courses. It will then determine whether the student passed or failed and prints on screen information. 

The code then sets up a socket connection between the producer and consumer using localhost. The producer sends the XML data over the socket connection to the consumer, which receives it and processes it. 

The authors are: 
1. Nandiso Shabalala (202101623 - B.Sc.IT)
2. Thandolwethu Shongwe (202102913 - B.Sc.IT)

Our Project voice-over demonstration video: https://youtu.be/1sxc4VE8bjQ


