# Metric
Metrics used for [[3-SLI]]

### Availability
The proposition of valid request served succesfully

- What is valid?
- What is succesful?

### Latency
The proposition of valid request served faster than a threshold

- What is valid?
- What is faster?
- what is a threshhold?

- What content are users are actually waiting for
- Careful when latency is being reported if at failure then missing time can't be account for
- Users care about when they queue the job, not when we acknowledge them and work on em.


### Quality
The proportion of valid request served without degrading service

- What is valid?
- How do we know content is degraded?

grading software needs to be able to check if a service is being degraded


### Freshness
Data is up to date and meet expectation of user

The proportion of valid data update more recently than a threshold

- When does recently mean? when does it start and stop 
-  What data is valid? 

### Correctness
The proportion of valid data produce correct output

- How to determine correctness
- What data is valid

### Coverage
The proportion of valid data processed sucesfully

- How to dermine if specfic piece of data is succesful

### Throughput
The proportion of time where the data processing rate (bytes/s)is slower than a threshold

- What is the threshold
-


