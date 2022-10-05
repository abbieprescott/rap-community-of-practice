# Over-engineering

Over-engineering can be defined as "the act of designing a product or providing a solution to a problem in an elaborate or complicated manner, where a simpler solution can be demonstrated to exist with the same efficiency and effectiveness as that of the original design". In other words, “When your design or code actually makes things more complex instead of simplifying things, you're over-engineering.”

Sometimes, when writing code, we add in unnecessary elements that don't contribute to the problem we are trying to solve, for example, adding code for a future problem ('just in case') or adding features that aren't part of the requirements. Both of these examples can be good things to do, however, if your team is under time constraints or your skills could be valuable somewhere else, it could be important to prioritise other tasks.

## What is over-engineering

It is important to weigh the opportunity cost. Compare whether working on the additional features or testing, for example, is preventing your team from working on something more valuable or whether the additional features/tests will reduce time spent completing this task again in the future.

This is an example table to help you to decide whether it is worth spending additional time to implement or make something more efficient:

![](../images/is_it_worth_the_time.png)

## Consequences

This is very dependent on the business area, for example, supporting a live service needs to be heavily engineered. Perhaps more so than code running a once a year publication as the cost of failure is lower if you only run the program once and can be fixed and run again without any impact on the service.

However, over-engineering often leads to higher business costs in the form of missing deadlines, lower team efficiency (if the team is delivering late), and potentially poor delivery of the product if it doesn't match the requirements. Additionally, a complex design or code could make the product cluttered and therefore could distract from the quality being produced. If you deliver complex code that is difficult to understand, your stakeholders or team members may struggle to use the code and therefore, take longer to understand or may not use it at all.

## Am I over-engineering

If you remove the feature you're adding and it doesn't affect your requirements/objectives, you're likely over-engineering.

This is a hard thing to judge as sometimes you might not be sure whether it will affect the requirement until you have implemented it. Additionally, the amount of time you spend designing or coding will be different for every feature so some things may seem more worth implementing than others as you can get them done sooner.

It is important to find a balance of how to implement your code based on, for example:

- Does it solves your problem?
- What is most important during delivery?
- What is the reason behind your approach - are there better alternatives?
- How simple it is to implement?
- Is it possible to simplify the feature?

When implementing code, often you get more benefit from focusing on implementing key functions, then you can go back and work to improve or refactor these when you have more time.

Your team may have a couple of key functions where you can implement tests to have most of the coverage. You could delay testing some one-off functions, or functions reused by other teams if there is a tight deadline. Your priorities will have to be decided by your team as your team may decide implementing really good code is more important than having an end-to-end pipeline sooner.

## How to avoid it

Firstly, it is important to have clear requirements or objectives for your project. You need a goal to be aiming towards to describe what features are key to include and therefore, you may not get as distracted implementing something unnecessary or over complex.

It is also important to define whether your project will be scalable. Some features may be required in the future and would be easier to add at the same time as another feature, however, some features could be noted as a future element and could be out of scope for the sprint you're working on. A problem with this could be that you focus either too much on the requirements you currently have and making more problems later if you have to refactor, or focusing too much on future elements and not including features that are required sooner than others resulting in missed deadlines. It is important to strike the right balance which is why you should discuss this with your team to make sure any requirements and objectives are clearly defined and possibly include a deadline for all the features.

Iteratively implementing your code is helpful when building your pipeline. Choosing one or a number of features, fixes or tests to work on in a Sprint (usually one to two weeks), helps to build your pipeline, keep track of what you are building, take into account any changes of requirements and fix any bugs as they arise. The team are able to constantly review the code and requirements and build on the pipeline.

Requirements often change and there are many ways to implement features however a reason why we publish our code in the open is so that we can peer review code and also reuse code. This helps to reduce over-engineering as you can focus only on the requirements that your team has and save time by reusing snippets of code that will help to make your code more efficient. Additionally, we can collect feedback from customers, stakeholders, or our peers to help improve our code and select the requirements more effectively. Another way to do this is by documenting your process. This can include making your code clear and easy to use, using [docstrings or comments][1] or creating a document to explain how to use the code and what its purpose is.

[1]: ../training_resources/python/python-functions.md#documentation
