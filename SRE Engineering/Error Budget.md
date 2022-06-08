# Error Budget
Error Budgeting ( EB ) are allowed errors to be served based on [[2-SLO]] and accepets the posbility of failure. The Biggest benifit of EB is it budgets the *time* 'to fail' , so we can afford to spend *time* on developing and creating  new features.

***Failure is acceptable and inevitable***

A system can't always be 100% reliable, however it dosen't mean we can compromise the reliability of a product for other features. So if reliability is a feature, how do we know which feature to take priority? Error budgeting is the solution for this!

## Creating an Error Budget
The best and most basic way to imagine a error budget is of course a allowance/budget. How much time we can spend on system failures. We can our expensives with the time left over from 9's systems.

| Time | Reliability   | Budget        |
| ---- | ------------- | ------------- |
| 28D  | 99.9% (3 9's) | 40mins of 28D |
| 1Y   | 99.9% (3 9's) | 8.77hrs of 1Y |

With a stable system with ***no changes*** we consistently have about 40min/month of room for failure or time to resolve TTR. 

***Majority of failures occur at release ( changes to system)***

Keep in mind an effective error budget can create:

- Common Incentive across team
- Self-Managed Risk
- balance development veolocity and reliability
- realistic goals 


## Responding to Error Budget
Error Budget main goal is to manage velocity and reliability, so depending of how how much we have, can trigger specific responses e.g:

- Push for new features
- Focusing effort 
- Reevaluate annd Review SLO
- Change [[3-SLI]]
  
Which can be dwindled down to responses to having:

- Leftover/Available Error Budget: Push/Develop more
- Exceeding/Meeting Error Budget: Halt development and divert focus to reliabilty

Which align to dynamic release cadences.

### Preventing Expenses
Exceeding Budget is a major indicator that development has superseded liability of a system and will require Engineering focus to system reliability. So how do we prevent expenses and impact? 

A general metric to determine expected impact of a specific failure is the porportion of Time-To-Detect plus Time-To-Resolve multiplied by the percentage of user impact over time between failures:

$$
\epsilon\sim\dfrac{(TTD+TTR)\times impact\%}{\Delta T}
$$

We try our best to keep expected impact close to miniscule amount and we can do that by editing any variable, such as a Canary Release which will reduce impact%. There is so much with ***expected*** failures, the rest main rely on operational service such as:

- Report uneven [[Error Budget]] in areas
- Provide input on achieving input (keeping x amount of changes with x amount of reliability)
- consult system design
- build safe releaseand rollback
- [[2-SLO]] violation produced post modem
- phased rollouts

There is an exception to the Error Budget rule which are silver bullets or critical features these silver bullets must be limited and are considered a failure and trigure a post modem


%%Error Budgect-based Alert%%
%%"Rainy Day Fund"%%





