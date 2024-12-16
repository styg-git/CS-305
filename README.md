# CS-305 - Software Security

**Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?**

Artemis Financial is a financial institution that wanted to use the most effective software security practices and techniques to improve and secure their RESTful web API.

**What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?**

I think the things I did well to address my client's security vulnerabilities were to implement industry best practices to avoid common threats. Addressing security vulnerabilities all begins with interpreting the client's needs and understanding their typical operations to know where the vulnerabilities may exist. I then did a manual review of the code to look for any glaring issues such as hardcoded information and areas where code could be better encapsulated. A suppression.xml file was added to suppress false positives as the dependencies for this assignment were pretty far out of date, but would not be fixed within the scope of this course. Finally, performing static and functional testing with the dependency-check information helped to "fill the gaps" regarding security vulnerabilities that were within my skill level to address. I believe utilizing the ciphers and hashing algorithms are areas where I excelled as I found them very interesting personally which always makes things more enjoyable to learn about.

**Which part of the vulnerability assessment was challenging or helpful to you?**

Initially, the most challenging part of the course was getting the tools configured and learning how to use them. Prior to this class I had heard of a pom.xml file, but never understand it's purpose or even what it would look like so getting some experience in working with one was helpful. Understanding how to use the different Maven build settings really streamlined things for me in terms of not needing to wait for 45 minutes for the dependency check to install every single time while still getting accurate information. Finally, being able to review the dependency check report to see various vulnerabilities within my code and suggestions for how to fix them was helpful and something I can see myself using in the future.

**How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?**

To increase layers of security, I limited the amount of information error provide to prevent any information from being misused to attack the system. I also enabled the HTTPS protocol, used a checksum, and the SHA-256 hashing algorithm to verify data integrity in a RESTful endpoint under localhost. Secure cryptographic practices ensure confidentiality and can tell you whether data has been compromised or tampered with. Encapsulation of sensitive data and methods within a program can help to prevent attackers from obtaining private information or learning too much about how a program functions.

**How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?**

The make certain that my code and software application were functional and secure, I utilized static and functional testing. 

**What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?**

Learning how to use the Maven Dependency check plugin was great for learning about potential vulnerabilities. I also learned some techniques to avoid exposing certain attack surfaces to bad actors throughout the course of working on the assignments. For example, simple practices like avoiding printing the stack trace directly to output, hard coding sensitive information, and sanitizing user inputs to prevent SQL injection and cross-site scripting can mitigate many potential threats.

**Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?**

I believe these assignments can showcase that I have at least a basic understanding of industry standard security practices. This was my first foray into cryptography and using dependencies, so I will definitely continue learning about those things to ensure the security of my personal projects. I also gained experience in creating self-signed certificates and learning some of the intracacies around that to prevent Chrome from throwing warnings and to fully enable the HTTPS protocol for secure communications. 
