# **Module-6-Concurrency**
## Commit 1 reflection
>: what is inside the handle_connection method. Write as reflection notes in 
the Readme.md
>>: the function uses a BufReader to read from the buffer instead of calling the OS, 
>>: then it wraps each stream into it, then giving an iterator of the lines in it.
>>: It iterates until it reaches an empty line then puts the results in the Vec
