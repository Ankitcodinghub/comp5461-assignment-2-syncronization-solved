# comp5461-assignment-2-syncronization-solved
**TO GET THIS SOLUTION VISIT:** [COMP5461 Assignment 2-Syncronization Solved](https://www.ankitcodinghub.com/product/comp5461-assignment-2-syncronization-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100022&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP5461 Assignment 2-Syncronization Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
• Specification.

</div>
</div>
<div class="layoutArea">
<div class="column">
In the first programming assignment, you have implemented the threads that allowed the operations of the client application and the server application to run concurrently. However, there were no critical section problem because only one server thread was updating the accounts and there was only one transaction on each account. In this programming assignment, the transaction file has been modified so that multiple transactions can be done on a single account. Therefore, if a thread blocks in a critical section while updating an account balance, then the result could be inconsistent if another thread also attempts another update operation on that account.

• Problem.

The Java code provided is similar to that of PA1 but there have been some changes to adapt it to the requirements of PA2 as shown below. For this assignment, the server will use two concurrent threads to update the accounts and thus we may have inconsistent results in case the critical section is not well protected. In addition, the synchronization of the network buffers (i.e. inComingPacket, outGoingPacket) is using busy-waiting so you need now to block a thread when a buffer is full or empty.

• Changes in PA1.

</div>
</div>
<div class="layoutArea">
<div class="column">
o

o

</div>
<div class="column">
UseofstaticmethodsinclassNetworkinordertocallthemethodsusing the class Name (i.e. Network) instead of using the instance variable objNetwork in classes Client and Server. Thus, the argument context in the constructor of the class Network is no more required.

Member variable serverThreadId in class Server identifies one of the two server threads. Member variables serverThreadRunningStatus1 and serverThreadRunningStatus2 indicate the current status of the two server threads. Also, the appropriate accessor and mutator methods have been added.

</div>
</div>
<div class="layoutArea">
<div class="column">
Winter 2021

</div>
<div class="column">
Page 1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
o Member variables of the Server class that have shared values with the two receiving threads are now static.

o A server thread is blocked in the deposit( ) method before updating the 10th, 20th, …, 70th account balance in order to simulate an inconsistency situation.

o Transaction file now includes two transactions for accounts in index positions 9, 19, … 69 (i.e. 10th, 20th, …70th accounts). Also, there are no transactions for accounts in positions 10, 20, …, 70.

• Implementation.

This problem will be implemented in two phases, phase (i) will synchronize the access to the critical section for updating the accounts and phase (ii) will coordinate the threads when accessing a full or an empty network buffer.

▪ Phase (i).

o First, you must adapt the Java code provided to your solution of PA1. In case your PA1 code doesn’t work properly, you will be provided help in the lab.

o Implement a second server thread in the main() method by respecting the changes already made in the constructor of the Server class. Consequently you need to modify the run() method of the Server class to accommodate the two threads and also to display the running time of each thread. The server can disconnect only when both threads have terminated.

o Now execute the program with DEBUG flags and notice the accounts with inconsistent results as shown in the file OS-pa2- output-unsynchronized.txt. The accounts 60520, 22310 and 91715 should be inconsistent but that may sometimes change depending on the sequence of execution. I have forced inconsistency by sleeping for 100 ms a thread accessing the critical section in the deposit() method of the Server class.

o Next, using synchronized methods or synchronized statements, protect properly the critical section of the methods deposit(), withdraw() and query(). Execute the program again and there should be no inconsistent results. Explain your choice of using either synchronized methods or synchronized statements.

▪ Phase (ii).

</div>
</div>
<div class="layoutArea">
<div class="column">
o

</div>
<div class="column">
The network buffers (i.e. inComingPacket, outGoingPacket) are synchronized using busy-waiting by constantly yielding the CPU until an empty buffer or a full buffer is available. This is good for the performance of the thread as it can respond quickly to the event but it is not good for the overall system performance as useful CPU cycles are wasted.

</div>
</div>
<div class="layoutArea">
<div class="column">
Winter 2021

</div>
<div class="column">
Page 2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
o Using the methods acquire() (similar to wait() or P()) and release() (similar to signal() or V()) of the class Semaphore, synchronize the operations of the network input buffers. The semaphores must be implemented in the methods send(), receive(), transferrIn() and transferOut() of the class Network. Sample output for this phase is in the file OS-pa2-output-semaphores.txt.

o Execute the program and comment about the running times of the server threads compared to using busy-waiting in phase (i).

• Sample output test cases.

o See attached text files.

</div>
</div>
</div>
