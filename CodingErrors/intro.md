# Intro to Coding Errors

## Overview
> **Computer security** is preventing attackers from achieving objectives through unauthorized access or unauthorized use of computers and networks [Howard 97]
* We aim to not allow unintended effects in our code\
-> Preventing hackers from using your device\
-> Preventing data leaks people could use 
* Security is the property of the software not the device
* **OpenSSL** a security protocol that causes buffer overflow\
-> Lead to the execution of arbitrary machine code\
-> Attackers could run code on your machine

> An **Exploit** is a piece of software that takes advantage of a security vulnerability to violate explicit or implicit security policy

## Side Effects
> C does not prevent memory from being written to the address of another variable
* Causes data corruption/crash
