# Designing Data-Intensive Applications

Short questionarie based on the book by Martin Kleppmann.

## Chapter 1. Reliable, Scalable, and Maintainable Applications

### 1. Differences between data-intensive and compute-intensive.
Compute-intensive demands computation work where most of their execution time is devoted to computational requirements
whereas data-intensive is a class of applications that use data paralell aproach to process large volumes of data (with size of tera or petabytes).

### 2. What are the caracteristics that make a system reliable? Mention an example of a not reliable system.
The reliability of a systems comes when it performs its intended functionality satisfactorily even under specific environmental and operating conditions. An example of the lack of system reliability lays in the failure either human, software or hardware made. For instance, a human mistake in the software that can create a series of cascading failures in a important component within the system.

### 3. Why rather to measure the performance of the system with percentiles than with mean?
Percentiles can more exactly measure the reachability in certain application. If you use the 99th percentile (p99) you can get the amount of users that reach that levels. In that way, you can fix anything needed. If you only use the mean, that gives you the average in your users and does not really tell you much information to fix anything.

### 4. What does make a system elastic? Give an example.
If a system is elastic, it means that it is able to add computing resources when detecting a load increase; for short, a system that is able to adapt to load changes. A clear example of it might be seen in cloud computing (AWS, Azure, Google Cloud), where you can choose what to pay according with your needs.

### 5. Therefore... What is the difference between scalability and elasticity?
Scalability gives you the ability to increase or decrease your resources (manually), and elasticity lets those operations happen automatically according to configured rules.

### 6. Does a one-size-fits-all scalable architecture exist? Why?
There is no generic architecture due to the problems with the volume of reads, writes and store, as same as the complexity of the data, the response time requirements, the access patterns, and more. Overall, the architecture of systems that operate at large scale is usually specific to the application to perform.

### 7. If you are working on the coding part of the development of a system for certain company, and you are part of the first version of the prototype, which maintainability design principle(s) you have to fulfill to avoid difficulties that you collegues might face?
Operability and simplicity. The former, to make it easy for operations teams to keep the system running smoothly, and the latter to make it easy for new engineers to understand the system, by removing as much complexity as possible from the system, avoiding a cascade of unnecessary failures.



