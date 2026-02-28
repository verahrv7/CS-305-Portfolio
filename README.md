# CS 305 – Software Security Portfolio

## Artifact Included
Project One – Artemis Financial Vulnerability Assessment Report

## Reflection

Artemis Financial is a financial services company that develops financial plans containing highly sensitive customer information such as investments, savings accounts, retirement accounts, and insurance data. The company required a security review of its RESTful web application to ensure that customer data remained confidential, secure, and protected from external threats. The primary issue addressed in this project was identifying vulnerabilities within the application and recommending mitigation strategies to prevent data breaches, injection attacks, and exploitation of outdated dependencies.

One area I performed well in was conducting a thorough manual code review and identifying multiple security weaknesses, including hardcoded credentials, lack of HTTPS enforcement, improper error handling, poor encapsulation, unvalidated input, and potential SQL injection risks. I also successfully integrated the OWASP Dependency-Check Maven plugin and analyzed 164 detected vulnerabilities across 13 dependencies. Coding securely is critical because financial institutions manage sensitive personal and financial data. Strong software security protects customer trust, prevents financial loss, ensures regulatory compliance, and strengthens a company’s long-term stability.

The most challenging part of the vulnerability assessment was interpreting the dependency-check results and determining which vulnerabilities required immediate prioritization. Many vulnerabilities were tied to outdated Spring Boot, Tomcat, SnakeYAML, Jackson, and Bouncy Castle dependencies. Learning how to assess severity levels and understand CVE documentation was particularly valuable in strengthening my analytical skills.

I increased layers of security by recommending HTTPS/TLS encryption, implementing input validation, securing database credentials, using prepared statements to prevent SQL injection, improving encapsulation, validating financial transactions, and upgrading vulnerable dependencies. In future projects, I would continue using static testing tools such as OWASP Dependency-Check, along with additional security scanning and code analysis tools to assess risks and determine appropriate mitigation strategies.

To ensure the software remained functional and secure after refactoring, vulnerability scans should be rerun after dependency updates, and regression testing should confirm that new vulnerabilities were not introduced. This layered approach strengthens both security and system reliability.

The tools and practices used in this project — including manual secure code review, OWASP Dependency-Check, Maven integration, secure coding principles, and CVE analysis — will be valuable in future coursework and professional development.

For future employers, this project demonstrates my ability to conduct a structured vulnerability assessment, analyze security risks, interpret CVE findings, prioritize mitigation efforts, and recommend secure coding improvements within a real-world financial application context.
