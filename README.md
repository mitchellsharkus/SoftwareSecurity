# CS 305 Portfolio

## Artemis Financial Vulnerability Assessment

### Client and Software Requirements

For this portfolio, I chose my Artemis Financial Vulnerability Assessment Report from Project One. Artemis Financial is a financial consulting company that creates financial plans for its customers, including savings, retirement, investments, and insurance. The company wanted to modernize its web application while also improving its security. My job was to look at the application and find security problems that could put the company or its customers at risk.

### What I Did Well

One thing I think I did well was looking at both the source code and the outside dependencies used by the application. During the manual review, I found problems such as the database username and password being stored directly in the code, the program using the root database account, missing HTTPS settings, input that was not being checked, and database connections that were not being closed. I also used OWASP Dependency-Check to look for known vulnerabilities in the libraries used by the application.

Secure coding is important because even a program that works correctly can still cause problems if an attacker can access information or take advantage of a weakness. Good software security helps protect customer information, keeps the application available, and helps a company maintain trust with its customers.

### Challenges and Helpful Parts

One of the more challenging parts of the vulnerability assessment was understanding the Dependency-Check report. The report found a large number of possible vulnerabilities, and at first it was difficult to tell which ones were the most important. It was helpful to learn how CVE numbers and severity scores can be used to understand the findings. I also learned that a tool finding a vulnerability does not automatically mean that the application can actually be attacked that way.

### Increasing Layers of Security

I increased the layers of security by looking at more than one part of the application. I reviewed the code, database access, user input, API endpoints, communication security, and outside dependencies.

If I was doing another vulnerability assessment, I would use tools such as OWASP Dependency-Check along with manual code review. I would start with critical and high-severity findings and then work down to lower-severity problems. I would also check for false positives so findings that do not actually affect the application can be documented and removed from future reports.

### Testing Functionality and Security

To make sure the application stayed functional and secure, I would test the application after making security changes and then run Dependency-Check again. This would help show whether the changes reduced the number of vulnerabilities and whether any new problems appeared.

I would also continue testing important parts of the application, such as the API and database connection, to make sure security changes did not break the original functionality. In this vulnerability assessment, I mainly reviewed and documented the existing code rather than doing a full refactor, but the same testing process would be important after refactoring the application.

### Resources, Tools, and Coding Practices

Some of the resources and tools that were useful during this project were:

- OWASP Dependency-Check
- National Vulnerability Database
- CVE information
- Oracle Secure Coding Guidelines
- OWASP Secure Coding Practices

I also learned that practices such as input validation, least privilege, protecting login information, using HTTPS, and keeping dependencies updated are important parts of secure development. These are tools and practices I can use again in future programming and cybersecurity assignments.

### What I Would Show Future Employers

For a future employer, I would show the completed vulnerability assessment report because it demonstrates that I can review an application for security problems, use a vulnerability scanning tool, read CVE information, and create a plan for fixing the problems I find.

It also shows that I understand that security is not only about making code work. Developers also need to think about how the software could be attacked and how to reduce those risks.
