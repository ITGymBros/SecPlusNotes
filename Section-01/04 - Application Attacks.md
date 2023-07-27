## Injections
- Supplying untrusted input
- Impact could be:
	- Loss of data
	- Corruption of information
	- Theft of information
	- DOS/DDOS

### Injection Types
- Structured Query Language (SQL)
- Lightweight directory access protocol (LDAP)
- Extensible Markup Language (XML)
- Dynamic Link Library (DLL)
- Command Injection

### SQL Injection
![Fileless](04_AA_Image_01.png)

### LDAP Injection
![Fileless](04_AA_Image_02.png)

### XML Injection
![Fileless](04_AA_Image_03.png)
- Would dump /etc/shadow file for password hashes

### DLL Injection
![Fileless](04_AA_Image_04.png)

### Command Injection
![Fileless](04_AA_Image_05.png)

## System Resources
- The components that provide its inherent capabilities and contribute to its overall performance; Internal tables and pointers set up to keep track of running applications
- Examples:
	- CPU
	- RAM
	- Disk I/O
	- etc...

### Resources and Memory
- Resource Exhaustion
- Memory Leaks
	- When an application is active and continuously consumes memory (NOTE: Might not always be an attack)

### Driver Manipulation
- Sophisticated attack
- Modification of driver functionality
- Exploits legitimate process

### Drive Manipulation Types
- Shimming
	- Small libraries
	- Perform actions
	- Legacy API support
	- Exploitable
- Refactoring
	- Modifying internal code
	- Behavior may not change
	- Design improvement
	 - Exploitable

## Race Conditions
![Race Conditions](04_AA_Image_06.png)

### Time of Check/Time of Use (TOC/TOU) 
- Example
	- Sue checks fileA.txt at 8:30 am
	- Bob modifies fileA.txt at 8:35 am
	- Sue starts to use fileA.txt at 8:40 am
	- fileA.txt is corrupted as it has 2 different version at the same time.
	- Integrity problem 

### Pointer / object Dereference
- Common in some programming languages (C/C++)
- Allows access to memory
- Code execution or denial of service

### Integer Overflow
![Integer Overflow](04_AA_Image_07.png)
- This flips the bits causing the integer to overflow
