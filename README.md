# Encryptus

You know how most Encrypt / Decrypt libraries and scripts are very complex, well i tried to keep mine as simple as possible!

Note: Please don't use this in an actual project, this is just a fun project i work on 🙂.

## How does it work?

Imagine that every letter has it's own number
	A: 1
	B: 2
	C: 3
Now let's take a random piece of text and convert every letter of the text into a number.
U would have something like '341213267', (well, just reverse it, duh!) I know, but first another problem:

Remember how the alphabet has more than 10 letters? 😮
This means that something like 10 11 12 could be interpreted as 1 0 1 1 1 2 wich only used the first 3 letters of the alphabet instead of the 10 till 12
To solve this problem we could start at higher values such as 100, now A starts at 100 and B at 101, great! now we need to add some sort of Encryption Key
Well, why dont we just Encrypt the key and add it to the already Encrypted text? Now we have a large number that fails to Decrypt, so to Decrypt it we just remove the (Encrypted) Key from the number and Decrypt it.

One problem i have been trying to figure out is Bruteforce Cracking, where you just get a random number to act like the Key and try to Decrypt it. One solution is to just make the Key long enough.
So i would recommend atleast 10-20 characters, the more the better but also the longer the Encrypted number will be.

Also, if this code or idea originates from any other program or library please make tell me, i dont want to copy other's work. 🫤
