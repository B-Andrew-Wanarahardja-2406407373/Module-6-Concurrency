# **Module-6-Concurrency**
## Commit 1 reflection
> What is inside the handle_connection method. Write as reflection notes in 
the Readme.md
>> The function uses a BufReader to read from the buffer instead of calling the OS, 
>> then it wraps each stream into it, then giving an iterator of the lines in it.
>> It iterates until it reaches an empty line then puts the results in the Vec,
>> then prints it out

## Commit 2 reflection
>> The newly added part is creating a response. with the code and length of 
>> hello.html as header, then it's contents as the body that gets shown. The 
>> images for the CLI at the time, and the response shown are in assets/images/

## Commit 3 reflection
>> This one makes it so that only the root path will show the hello.html (it matches
>> if request is GET / HTTP/1.1, the '/' after GET is the root path), otherwise it 
>> will show the not found page. The CLI at the time and the bad page is also in
>> assets/images/