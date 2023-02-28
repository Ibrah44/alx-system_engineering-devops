<img src=./image.png width=50%>

# BooktifuL requests failure report
 On March 1, 2023, between 1:00 PM to 3:30 PM EST, our web application experienced an outage that impacted all users. The root cause of the outage was a misconfigured database setting that caused a bottleneck in our system, resulting in slow page loading times and intermittent errors for all users.

## Timeline
1:00 PM: The issue was detected through an increase in user complaints to our customer support team.
1:05 PM: Our engineering team was alerted through our monitoring system and began investigating.
1:15 PM: Investigation began with a focus on server and network issues as they were the most likely culprits.
1:30 PM: Misleading investigation paths led us to focus on a recent code deployment as a potential cause, and we began rolling back to a previous version.
2:00 PM: Despite the rollback, the issue persisted, and we expanded our investigation to the database.
2:30 PM: Our database team discovered a misconfigured setting that was causing a bottleneck.
2:45 PM: The incident was escalated to our senior engineering team.
3:00 PM: The root cause was identified and fixed, and the application was restored.
3:30 PM: Normal application functionality was fully restored, and the incident was declared resolved.

## Root cause and resolution
The root cause of the issue was a misconfigured database setting that caused a bottleneck in our system. Specifically, the database was set to use a limited amount of memory, which resulted in slow queries and a buildup of connections that overwhelmed the system. Our database team resolved the issue by increasing the memory allocation and optimizing the database's configuration to prevent a recurrence of the problem.uests.

## Measures against such problem in future
To prevent similar issues from occurring in the future, we will implement the following corrective and preventative measures:

- Increase our monitoring capabilities to detect similar issues earlier.
- Establish clearer protocols for escalation and communication during incidents.
- Improve our testing procedures to catch misconfigurations during deployment.
- Increase the frequency of database performance reviews to identify and address bottlenecks before they cause outages.
- Train our engineering team to recognize and address database issues more quickly and effectively.