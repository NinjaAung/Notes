# Service Level Objective
A Service Level Objective ( SLO ) are measurable internal objectives we can meet in a [[1-SLA]]. The biggest benifit of SLO, is to sync teams and provide a clear achievable objectives to meet SLA and User Satisfacation.

***Achievable SLO is not 100%***

Failure is normal and systems can afford to fail. If we to direct all effort into realability, how can new features be deveoped? So how can we create an effective SLO to balance relability, development and user satisfaction while budgeting our failures?

## Creating a SLO
SLO are the diving line of happy and unhappy customers, so our goal is to achieve better than the [[1-SLA]]. However a SLO baseline will always be the [[1-SLA]] —'the minimum requirement'. SLO's are stronger than SLA to prevent the oppurtunity to violate [[1-SLA]] and keep users happy.

***It's always better to under promise and over deliver***

Keep in mind a achievable SLO is only effective if they:

- Are within the desirable range of users
- Have Executive Buy-In
- Are Accurently Measured
- Have Consequences

Example of internal achievable SLO vs SLA:

![[SLO_Balance.png]]

Now that we have a general idea of what is an *achievable* SLO, we create SLO with every service of interest keeping in mind quality > quanity. Finally we need [[3-SLI]] metrics to compare against. Finally SLO need to always be re-reviewed all the time

### What's The Benifit?
An effective SLO can provide a healthy balance of performace reliability and developing new features. Pushing a feature should not or continue to violate a systems reliability. If a SLO isn't being reached it should either be:

1. Prioritize for Engineering effort
2. Reavulated

### Reavulating a SLO
SLO can be divided into achievable and aspirational they can occasionally diverge, but it's best to clarify:

- Achievable: SLO based on past performance
- Aspirational: SLO based on business needs

A SLO should be continous developed and updated, should change at most within a year.

### Responsible For 
- Setting customer expectations and teams what metrics we are looking for and what to measure them against
- Prioritizing features and pacing development not at the expense of users ( **Reliability is a feature!** )
- Determining the right level ofr eliability
- Understanding and creating error budget ( [[Error Budget]] )
