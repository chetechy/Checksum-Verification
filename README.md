# Checksum-Verification
Overview
Two people working on a computerThe cryptographic hash function is very useful for sharing information. When an organization needs to distribute programs or documentation to customers, the organization can use the hash value to make certain the customer receives unchanged information. When you produce a hash value for a data file, it is called a checksum. If you produce a checksum for files that customers will download, then your customers can check for transmission errors. It also prevents an attacker from disguising a malicious file as your original file.

To prevent these attacks, you’ll need to produce a cryptographic hash function that is not susceptible to collisions. For example, some older algorithm ciphers have been found to be hackable. In other words, a hacker can produce a checksum for a malicious version of a file that equates to the same checksum as the original file. In this assignment, you’ll need to research options to find and produce a cryptographic hash function that will not be susceptible to collisions. You’ll deploy an appropriate algorithm cipher to encrypt and produce a checksum verification to increase the security layers for a software application.

Directions
A business you are working with has a public key that they are hoping to distribute to clients. Their clients want to download the public key from a website and verify the key with a checksum. To accomplish this, you will need to code a simple string checksum verification program. In addition, you will need to document your process by completing the Module Five Coding Assignment Checksum Verification Template, linked in What to Submit.

Specifically, you must address the following rubric criteria:

Algorithm Cipher: Recommend an appropriate encryption algorithm cipher that avoids collisions.
a. To do so, review the scenario and the Java Security Standard Algorithm Names, which is a standard list of algorithm ciphers provided by Oracle.
b. Document your recommendation in the template provided.

Justification: Justify your reasoning for the recommended algorithm cipher that avoids collisions.
a. To do so, provide a brief, high-level overview of the encryption algorithm software. Consider what it means to avoid collisions. Why is this important?
b. Document your reasoning in the template provided.

Generate Checksum: Refactor the code to encrypt a text string and generate a checksum verification.
a. To do so, first download the Module Five Coding Assignment Checksum Verification Code Base, linked in the Supporting Materials section, and upload it to Eclipse as a new project. Refactor the code to add your first and last name as a unique data string. You will submit your refactored code for your instructor to review. Then generate the checksum by following these steps:
1. Create an object of MessageDigest class using the java.security.MessageDigest library.
2. Initialize the object with your selection for an appropriate algorithm cipher.
3. Use the digest() method of the class to generate a hash value of byte type from the unique data string (your first and last name).
4. Convert the hash value to hex using the bytesToHex function.
5. Create a RESTFul route using the @RequestMapping method to generate and return the required information to the web browser, including the hash value.

Verification: Demonstrate that a hash value has been created for the unique text string (your first and last name) by executing the Java code.
a. Then use your web browser to connect to the RESTful API server. It should show your first and last name as the unique data string in the browser, the name of the algorithm cipher you used, and the checksum hash value.
b. Capture a screenshot of the web browser with your unique information and add it to the template provided. An example of the expected output is shown below:
