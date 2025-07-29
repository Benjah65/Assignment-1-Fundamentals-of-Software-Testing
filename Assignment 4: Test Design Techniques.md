🧪 Assignment 4: Test Design Techniques

Submitted by: Benjamin (Dummy 😎)
1. Define black-box and white-box testing. Provide at least 2 differences between them.

Black-box testing is a technique where the tester does not need to know the internal structure of the code. Instead, they focus on testing the software from the user’s perspective—inputs, outputs, and behavior.

White-box testing is where the tester has full knowledge of the internal workings of the application. It involves testing the code logic, paths, and structures.
Black-box Testing	White-box Testing
Tester doesn't see the code	Tester sees and analyzes the code
Focuses on what the software does	Focuses on how the software works
Done by QA or testers	Often done by developers
Example: testing a login form	Example: testing if an if statement works as expected
2. Using Equivalence Partitioning, create test cases for a login system where:

    Username must be between 4–12 characters

    Password must be at least 8 characters

Equivalence Partitions:
Input	Valid Partition	Invalid Partition
Username length	4–12 characters	<4 or >12 characters
Password length	≥8 characters	<8 characters

Test Cases:

    Username: "user1" (5 chars), Password: "password" → ✅ Valid

    Username: "ab" (2 chars), Password: "password" → ❌ Invalid (short username)

    Username: "thisisaverylongname" (17 chars), Password: "password" → ❌ Invalid (long username)

    Username: "ben123", Password: "1234567" → ❌ Invalid (short password)

    Username: "joyful", Password: "hello1234" → ✅ Valid

3. Apply Boundary Value Analysis for the same login system.

Boundary values:

    Username: 3 (invalid), 4 (valid), 12 (valid), 13 (invalid)

    Password: 7 (invalid), 8 (valid)

Test Cases:

    Username: "usr" (3 chars), Password: "password" → ❌ Invalid username

    Username: "user" (4 chars), Password: "password" → ✅ Valid

    Username: "longusername" (12 chars), Password: "password" → ✅ Valid

    Username: "toolongusername1" (13 chars), Password: "password" → ❌ Invalid username

    Username: "validname", Password: "1234567" → ❌ Invalid password

    Username: "validname", Password: "12345678" → ✅ Valid

4. Create a Decision Table for an online store checkout:
Condition	Rule 1	Rule 2	Rule 3	Rule 4
Has coupon?	Yes	Yes	No	No
Cart total > $50?	Yes	No	Yes	No
Discount applied	20%	10%	5%	0%

Explanation:

    Rule 1: Best case → coupon + big cart = 🤑 20% off

    Rule 2: Only coupon = 🧾 10% off

    Rule 3: Only big cart = 💰 5% off

    Rule 4: No coupon, small cart = ❌ no discount

5. State Transition for user registration:

States:
Start → Enter Info → Verify Email → Account Created

Valid Transitions:

    Start → Enter Info

    Enter Info → Verify Email

    Verify Email → Account Created

Invalid Transition Example:

    Start → Verify Email (❌ Can’t verify before entering info)

6. How do test design techniques improve software quality and reduce bugs?

Test design techniques make testing smarter, not harder. Instead of testing every possible input (which is impossible), they help you pick the most effective test cases. Techniques like Equivalence Partitioning and Boundary Value Analysis find bugs near the edges—where things often break. Decision tables and state transitions help you test logic and workflows better. All of this means fewer bugs, less stress, and better user experience. 💯
