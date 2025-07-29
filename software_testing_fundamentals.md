Assignment 1: Fundamentals of Software Testing
1. Importance of Software Testing in Software Development

Software testing is a critical step in the software development process because it ensures the quality, reliability, and performance of an application. It helps in identifying bugs and issues before the product reaches the end user, saving time, money, and reputation. Testing also ensures that the software meets the specified requirements and behaves as expected under different conditions.
2. Differentiate between Errors, Defects, and Failures

    Error: A human mistake made during coding, designing, or requirement gathering. For example, using the wrong variable name in code.

    Defect (Bug): A flaw found in the software code, usually caused by an error. It’s something wrong in the implementation.

    Failure: When a defect is executed and causes the software to behave incorrectly or crash in real use, it's called a failure.

Example:
If a developer forgets to handle null input (error), the app crashes when a user submits empty data (defect), leading to a crash in production (failure).
3. Explain the Pesticide Paradox

The Pesticide Paradox in testing means that running the same set of tests repeatedly will eventually stop finding new bugs. Just like using the same pesticide repeatedly stops working on pests, relying only on fixed test cases won't catch newly introduced bugs.

To overcome this, testers must regularly update and add new test cases to explore different parts of the software and catch more issues.
4. Static Testing vs. Dynamic Testing
Feature	Static Testing	Dynamic Testing
When it's done	Before code is run	After code is run
What it checks	Code, documents, and design	Actual behavior of software during execution
Examples	Code reviews, walkthroughs	Unit tests, integration tests
Cost-effectiveness	More cost-effective (early in SDLC)	Less cost-effective (post-coding phase)

In simple terms: Static testing = checking the code on paper. Dynamic testing = running the code and seeing what breaks.
5. Why Testing Should Start Early in the SDLC

Testing early in the SDLC (like during planning and designing) helps catch errors when they are cheaper and easier to fix. The later a bug is found, the more expensive it becomes to correct.

Early testing = less rework, faster development, and better product quality. It also ensures that the design and requirements are testable and feasible from the start.