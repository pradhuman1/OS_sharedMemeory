# OS_sharedMemeory

Given Proect contains following Solution :
Implement a solution to the bounded-buffer producer-consumer problem using only two shared
variables ‘in’ and ‘out’ (apart from the shared buffer itself), which indicate the positions in the buffer
array where / from where the next item to be inserted / retrieved by the producer and the consumer
process respectively. Note that in this solution, the buffer can contain maximum (BUFFERSIZE-1) items.
In your solution, do not use busy waiting based iterative loops (as shown in book), rather, use the pause()
and kill() system calls to block and unblock a process as demonstrated in my example programs / videos.
Note that, in this solution, although in and out are shared variables, none of them are updated by multiple
processes, rather, in is updated only by the producer process and out is updated only by the consumer
process. Hence, we do not need to synchronize the access of these two shared variables.
Now, implement the following on the top of the above solution:-
Producer process, on each iteration, takes details of a student (name, enroll no, section, age etc.)
from the user and puts this data as an item into the shared buffer. The consumer process on the other
hand, on each of its iteration, retrieves a data item from the buffer and saves it in a CSV file on the disk,
where the fields (name, enroll no. etc.) of a data-item are stored in comma-separated format (as usually
stored in CSV).
