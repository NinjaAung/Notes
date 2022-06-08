# Service Level Indicator
A Service Level Indicator ( SLI ) are [[Metrics]] based on the performace for a [[2-SLO]]. The biggest benifit of SLI is they can provide evidence of User Experince that can drive or halt development across teams.

***User experince is always right, regardless of percieved SLI metric.***

Even if SLI's have positive metrics, a developer challenges dwindle down to user percieving the website is simply not working ( User sad `:(` ).  So how do we record SLI?

## Recording SLI's
SLI are measured by the proportion of `good events` to `valid events`. It's also important to know which metric is a good event. Good events are described as:

- Having *almost* linear relationship of sys operations to clients happiness over time
- Depicting long-term trends clearly (low noise)
- Showing service is working as users expect them to

Example of metric:

![[SLI_Trends_In_Operation.png]]
 
 
 
## Choosing a Indicator
There are lots of [[Metrics]] to use, so it's good to know where and what to use those with.  Avaliability, Latency, Quality, Freshness, Coverage, Correctness, Througput and Durability are all possible indicators of SLI. Instead of being overwhelmed with all of them it's good to choose from indicator frequently used with a service. 

***Quality over quanity, the quantity of SLI will backfire in a slowdown***

### SLI Menu
Here is the SLI menu a kinda quick start guide of the most frequent use of each metric. Then the depth of the indicator can further be specified at [[Levels Of SLI]]. _The menu is not a strict use of SLI's_

| Service         | What To Track                                   |
| --------------- | ----------------------------------------------- |
| Req / Resp      | Availability, Latency and Quality               |
| Data Processing | Freshness, Coverage, Correctness and Throughput |
| Storage         | Durability                                      |
|                 |                                                 |


## SLI In Practice
With the menu, we can knock obviouse use cases, like making sure content is loading quick and now produce a clear [[2-SLO]]. So keep in mind to:

1. Define SLI in high-level terms
2. Refine SLI into detailed implementation
3. Walkthrough userjourney and look for coverage gaps
4. Set SLO

SLO [[Metrics]] can be expressed as: 
	The portion of ==def_of_events== to ==param== measured at ==point of interaction==

Example:
	Availability: The portion of ==valid_request== that were ==served_sucessfully==
	valid_request: HTTP GET request for `/user` 
	served_succesfully: 2xx,3xx or 4xx response code
Final:
	The portion of ==HTTP GET request for /user== that have ==2xx,3xx or 4xx response code== measured at ==load balancer==




