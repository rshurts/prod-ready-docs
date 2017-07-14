# Runbooks

Provide troubleshooting guidance for the product's alerts in runbooks. Each runbook should include the alert name, a description of the alert, a description of the problem the alert indicates, and step-by-steps instructions to triage, mitigate, and resolve the alert. In addition, the runbook should detail any business and user facing impact the alert signifies along with how to communicate the incident to the team or broader organization.

General troubleshooting and debugging guidance, on-call requirements, and on-call procedures should also be provided in this section.

> **Write Runbooks that Developers Can Follow at 2AM**
>
> Use clear concise language and explicitly write out any commands so a sleepy developer responding to an alert can easily follow along and resolve the alert. The last thing you want are poor instructions that result in taking a bad situation and making it worse.


#### Example


### Procedure

- Post to `#prod-ready-docs-dev` in Slack that you are responding to an alert using the alert's name.
- Follow the instructions in the runbook to triage, mitigate, and resolve the issue.
    - If the issue isn't resolved call the person on the on-call escalation rotation.
    - Use the [Troubleshooting and Debugging](runbooks.md#troubleshooting) section to help resolve the issue.
- Post to `#prod-ready-docs-dev` in Slack that the alert has been resolved using the alert's name.
- The following business day, create a post-mortem document and schedule a post-mortem review with the team.


### Troubleshooting and Debugging {#troubleshooting}

- [Have you tried turning it off and on again?](https://www.youtube.com/watch?v=nn2FB1P_Mn8)


### Alerts

- [Order 66](order-66.md)
