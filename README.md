# PwnedPasswordsChecker

This project is a small Python script that uses the Have I Been Pwned API for safely checking whether a password has been pwned, without sharing it, or its hash. Instead, it sends the first 5 characters of the hash and the API sends back all hashes that start that way. This script then checks whether your hash is in the response.

In the Computerphile video "Have You Been Pwned?", Dr Mike Pound uses a script exactly like this one to check how many times certain passwords had leaked in a safe manner. He didn't release the source code (as I'm writing this) and many people wanted the script, so I made a quick implementation. The video: https://www.youtube.com/watch?v=hhUb5iknVJs

How to use:

- Use Python 3
- Before running the script, download the requests Python module by going into CMD and typing "pip install requests"
- Use the script by calling it this way in CMD: python pwned.py PasswordToCheck
