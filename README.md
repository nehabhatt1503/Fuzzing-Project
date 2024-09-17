# Fuzzing-Project
Fuzzing or fuzz testing is an automated software used to test error handling of the software by providing invalid, unexpected, or random inputs.

---

## Terminologies:
### Wordlists: Wordlists are text files containing a sequence of commonly used words. This can be lists of common user names, passwords, website directories, typical files on a website, etc.
### SecList: One of the most comprehensive and widely-used collections of wordlists is SecLists. 
#### SecLists contains wordlists for:
- Common directory and file names
- Backup files
- Configuration files
- Vulnerable scripts

### ![image](https://github.com/user-attachments/assets/4100ebb9-2ccc-4c8f-a9a0-7dfbd9a56156)
### ![image](https://github.com/user-attachments/assets/7de63969-e7cd-4878-8c44-61c3c053c6f3)


### Fuzzer: A software tool that automates generating and sending payloads to a web application and analyzing the responses. Example- ffuf, wfuzz, Burp Suite.
--- 


The most commonly used wordlists for fuzzing web directories and files from SecLists are:
#### ![image](https://github.com/user-attachments/assets/0af59fda-3561-4bf7-b432-6d97ae74b04e)



## How ffuf generally works:
1. Wordlist: You provide ffuf with a wordlist containing potential directory or file names.
2. URL with FUZZ keyword: You construct a URL with the FUZZ keyword as a placeholder where the wordlist entries will be inserted.
3. Requests: ffuf iterates through the wordlist, replacing the FUZZ keyword in the URL with each entry and sending HTTP requests to the target web server.
4. Response Analysis: ffuf analyzes the server's responses (status codes, content length, etc.) and filters the results based on your criteria.




