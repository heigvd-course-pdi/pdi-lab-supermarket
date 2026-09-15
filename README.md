Optimization of a Supermarket Checkout System
=============================================

In this lab you will use queueing theory and discrete-event simulation to analyze and optimize the checkout system of a supermarket.

The learning goals of this lab are:

- to apply queueing models such as M/M/1 and M/M/c to a real-world system,
- to write SimPy simulation models,
- to understand the performance characteristics of the different queueing models.

Problem description
-------------------

The management of a supermarket wants to design an efficient system to organize the checkout of customers at the cash registers. The management considers the following options:

- **Separate queues**: 5 cash registers, each with its own queue. The customer chooses a queue when he arrives at the checkout area. It is assumed that they do not switch queues.
- **Single queue**: 5 cash registers, with a single queue. The next customer in the queue goes to the next available cash register.
- **Robot cashier**: a single cashier (robot) that is 5 times faster than a human cashier.

### Assumptions

- The service times are exponentially distributed, with a mean service time of 100 seconds for a human cashier. The robot cashier is 5 times faster, i.e., has a mean service time of 20 seconds.
- The arrival process of customers is Poisson. The arrival rate may vary during the day from 0.1 to 2.7 customers per minute.

### To do

- Develop a simulation model for each of the three options using SimPy. 
- Write simulation scripts that run the models for different arrival rates and generate plots of the mean total time for checkout (waiting time + service time).
- Compare the results of the three options for low, medium, and high arrival rates.
- Answer the questions in the file `Questions.md`.

You can reuse and adapt scripts and models from previous labs.
