# Trunk-based development (TBD)

Trunk-based development (TBD) is a software development approach that emphasizes continuous integration and delivery by keeping a single codebase (known as the trunk or mainline) that is always in a deployable state. This approach requires developers to commit their changes to the trunk frequently and encourages them to keep their code small and focused.

In a typical TBD workflow, developers start by checking out the latest version of the trunk and creating a new branch to work on their changes. They then work on their code in isolation, committing their changes to their branch as they go. Once they have completed their changes, they submit a pull request or merge request (depending on the version control system) to merge their changes into the trunk.

Benefits…

* Faster feedback and testing: By keeping the codebase in a deployable state, teams can quickly test and validate changes, reducing the time it takes to get feedback and make adjustments.

* Increased collaboration: TBD encourages developers to work together and share code frequently, leading to improved collaboration and knowledge sharing across the team.

* Better code quality: The continuous integration and delivery approach of TBD helps to identify issues early in the development process, leading to better code quality and fewer bugs.

* Faster time to market: By quickly validating changes and identifying issues early in the development process, teams can release new features and updates more quickly, reducing time to market.

However, trunk-based development has challenges. One potential issue is when multiple deployable versions are necessary, such as via long-lived release branches, or via multiple on-premise deployments to customers.
