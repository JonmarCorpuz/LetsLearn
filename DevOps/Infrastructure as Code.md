# Infrastructure as Code Oververview

IaC is the practice of automating and managing infrastructure using reusable scripts

* Made possible through the use of APIs
* Replaces the time consuming and expensive manual provisioning of infrastructure
* Supports an immutable environment where the outdated resources are replaced with an updated version instead of merely patching the issue
* Saves costs by freeing developer time to docus on other projects
* Eliminate the risk of human error by avoiding manual configuration
* Provides faster and more efficient development by allowing teams to deploy and work on the same infrastructure throughout the software development lifecycle
* Reduces configuration drift by enforcing consistency through and using one configuration file as the single source of truth (When a resource's configuration has altered from its original or expected state due to unplanned changes to the configuration code or unmonitored software or hardware updates)
* Increases accountability since storing the configuration files within a single repository increases visibility into changes made to the configuration code

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# IaC Programming Models

## Declarative

* Users define the system's desired state from the start
* IaC tools first look at the current state of the infrastructure and then makes the appropriate changes to achieve the desired state for them

## Imperative