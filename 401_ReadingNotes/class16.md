# Class 16 Reading Assignment

## What is Serverless Computing?

Serverless is a cloud computing application development and execution model that enables developers to build and run application code without provisioning or managing servers or backend infrastructure.


The name notwithstanding, there are most definitely servers in serverless computing. 'Serverless' describes the developer’s experience with those servers—they are are invisible to the developer, who doesn't see them, manage them, or interact with them in any way.



Function-as-a-service, or FaaS, is a cloud computing service that enables developers to run code or containers in response to specific events or requests, without specifying or managing the infrastructure required to run to code.

Provisioning: 
time Measured in milliseconds for serverless, vs. minutes to hours for the other models.

Administrative burden:
 None for serverless, compared to a continuum from light to medium to heavy for PaaS, containers and VMs respectively.

Maintenance: 
Serverless architectures are managed 100% by the provider. The same is true for PaaS, but containers and VMs require significant maintenance including updating/managing operating systems, container images, connections, etc.

Scaling: 
Auto-scaling—including auto-scaling to zero—is instant and inherent for serverless. The other models offer automatic but slow scaling that requires careful tuning of auto-scaling rules, and no scaling to zero.

Capacity planning: 
None needed for serverless. The other models require a mix of some automatic scalability and some capacity planning.

Statelessness: 
Inherent for serverless, which means scalability is never a problem; state is maintained in an external service or resource. PaaS, containers and VMs can leverage HTTP, keep an open socket or connection for long periods of time, and store state in memory between calls.

High availability (HA) and disaster recovery (DR): 
Both are inherent in serverless with no extra effort and at no additional cost. The other models require additional cost and management effort. In the case of both VMs and containers, infrastructure can be restarted automatically.

Resource utilization: 
Serverless is 100% efficient because there are no such things thing as idle capacity—it is invoked only upon request. All other models feature at least some degree of idle capacity.

Billing granularity and savings: 
Serverless is metered in units of 100 milliseconds. PaaS, containers and VMs are typically metered by the hour or the minute.

Kubernetes is an open-source container orchestration platform that automates the deployment, management and scaling of containers. Kubernetes' automation dramatically simplifies the development of container-based applications.

### Things I want to know more about

### References

https://www.ibm.com/topics/serverless