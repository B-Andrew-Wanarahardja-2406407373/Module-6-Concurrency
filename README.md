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

## Commit 4 reflection
>> By using only a single thread, if multiple users want to access the site and one
>> of the users are slow, then the others that follow will not be able to access it
>> until the slow user got through, simulated by the thread sleeping for 10 seconds.
>> when one accessed 127.0.0.1:7878/sleep and after that another accessed 
>> 127.0.0.1:7878, the latter was not able to access the site until the 10 seconds 
>> of the former was over