# cafeteria_simulation
Simulation of dosa(food court) queue at IIT(BHU) cafeteria to decrease the average waiting time of customer to less than 6 minutes. 

This was a coursework project under our professor at Indian Institute of Technology(BHU), Varanasi. The objective was to simulate the customer waiting at dosa (a south indian cuisine) counter, to reduce there average waiting time below 6 minutes. Realtime data was collected by measuring the inter-arrival time, serivce time at cash counter, proportion of customers asking for dosa, service time at dosa counter, all at peak hour of 12:00 p.m. to 2:00 p.m. The waiting time at dosa queue was also measured for hypothesis testing i.e. correctness of simulation. Then a parallel dosa counter was simulated for the effect on waiting time. 

Tools: Arena simulation software

#Steps for measurement

1. The arrival time of customers in the cash counter queue was measured using a stopwatch and calculating the time difference between two arrival instances is inter-arrival time.
The arrival instance is created as soon as the person joins the queue.
2. The service time per customer at cash counter was measured by measuring the the time difference between the instance that the customer arrives at the cash window and the instance of leaving the cash window. 
3. The proportion of dosa consumers were evaluated by taking the ratio of total dosa orders & total number of requests inbetween peak hhours.
4. The service time per customers was measured by measuruing the time difference between the customer arriving at order window and leaving the window. 
5. The waiting time of customers in dosa queue was measued using the time diffrence between the customer joining dosa queue and customer arriving at the order window.
6. The time difference between two failures at dosa counter and cash counter was also measured along with the failure time.
7. The number of peoople in dosa queue at the instance of beginning of peak hours were also measured for seven days and the condition was added as 'queue clearance initially' in simulation model. 

Assumptions:

1. The customers don't leave the queue after joining it(no reneging).
2. The customer requesting for dosa joins the dosa queue directly after leaving cash window.

The histograms for service time, inter arrival time and waiting time were plotted for statistical analysis and were modeled using Arena. The actual mean waiting time and simulated were validated using hupothesis testing for the correcteness of simulation with 95% confidence interval. The effect of adding a parallel dosa counter on mean waiting time of customers was simulated assuming identical service time distributions of both counters.

* True mean waiting time: 8.3 minutes
* Simulated mean waiting time with single dosa counter for 30 replications: 8.93 minutes
* Simulated mean waiting time with parallel dosa counter for 10 replications: 2.44 minutes
