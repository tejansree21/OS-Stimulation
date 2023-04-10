# OS-Stimulation
This is a C program which implements two scheduling algorithms namely fixed-priority scheduling and round robin scheduling algorithm

The program starts by asking the user to input the number of processes for priority scheduling.
Then for each process it takes process name, process time and process priority. This data is stored in arrays 'p', 'pt', and 'pr' respectively.
The program then sorts the processes according to the priority using a nested loop and a temporary variable to swap values
After sorting the program calculates the waiting time of each process based on the pervious process's waiting time and adds it to the total waiting time

The program then asks the user to input number of processors for round robin scheduling, followed by the time slice for the processess
For each processes it asks for the process ID and brust time. Then the program initializes an array for the remaining time and another array for the processes waiting time. It then uses a loop to execute the processes based on the time slice and remaining time 
If a process remaining time is greater than the time slice it subtracts the time slice and updates the waiting time for other processes. Otherwise it sets the remaining time to 0 and updates the waiting time and turn arround time. After executing all the processes the program calculates the average waiting time and average turn around time
The average waiting time and average turnaround time are calculated using the formulas awt = total wait time/number of processes and atat = total trunaround time/ number of processes respectively.
Finally the program outputs the details of each process for both scheduling algorithms along with the total waiting time and average waiting timefor round robin scheduling.
The results are then printed on the screen using printf statements
