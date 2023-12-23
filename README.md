Java URL Shortener Program
This Java program provides a basic command-line interface for a URL shortener. It allows users to store URLs, retrieve short keys, count usage, list all URLs with counts, and exit the program.

Usage
To start the program:


java URLShortenerProgram


Available Commands:

storeurl <URL>: Store a URL and generate a unique short key.
get <URL>: Retrieve the unique short key for a given URL and increment the usage count.
count <URL>: Retrieve the latest usage count for a given URL.
list: List all stored URLs with their usage counts (JSON format).
exit: Terminate the program.
Example Commands:

bash
Copy code
storeurl https://www.example.com
get https://www.example.com
count https://www.example.com
list
exit


Implementation Details
The program uses local variables to store data instead of a database.
A combination of the current timestamp and a counter is used to generate unique short keys.
URLs and their usage counts are stored in a simple HashMap.
The program continuously waits for user commands until the exit command is entered.
Author
[Rohit Kumar]
