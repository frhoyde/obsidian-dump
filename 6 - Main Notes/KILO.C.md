##  30.06.26 ~ 21:57 
---

>[!note] I have created a make file of one line to compile this thing. Apparently C17 still has support for c99. Although I thought about switching to -std=c17 (I don't know if it would've worked or not) but I decided to keep going with c99 because it still is supported by this gcc version 13.3

- read() reads 1 character at a time. but in "buffer"
- [[Terminal - Canonical Mode]] is not good for our task. We need to enter raw mode for this for smooter editing capabilities.

>[!note] I think I was kind of asking good questions. One of them was, when we're reading and setting terminal attributes, why are we using pointers or the pass by reference for the termios struct? I even wondered,  I could theoretically use return values and use the normal pass by value feature. It's because tcgetattr and tcsetattr also return an integer, 0 or 1 based on the success or failure of the operation.

>[!note] So what is a file descriptor? A file descriptor is basically specifying a channel, a fixed and known slot that the process agrees to treat.

- STDIN - 0
- STDOUT - 1
- STDERR - 2
- all FDs have the same interface - read(), write(), close()

> [!note] TCSAFLUSH is responsible so that button mashers can mash buttons freely. So, whenever we're starting raw mode, and while starting, if we mash buttons, those input keystrokes are "flushed"

>[!note] Also We are disabling ECHO because we are going to manage that manually, giving ECHO the freedom to dump characters anywhere can cause issues to our manual way. It might double render as well

>[!note] The ICANON flag holds all the keystrokes in an internal line buffer. It only gives this input over to read() once the ENTER key is pressed. Turning it off gives us the flexibility to read input character by character or byte by byte instead of going line by line.
>


