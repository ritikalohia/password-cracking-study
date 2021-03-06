password-cracking-study
=======================
Overview
--------
<p>Any company or organisation wants their costumer data to be secured and non-rerachable to hackers.If 
company's data gets hacked, and the database leaked in public. database can be misused. It  spoils 
the image of a company and make it untrustworthy. That's why, any organisation wants to be a step ahead 
of hacker, in order to prevent important database from hackers. We need to know the techniques used by 
the hackers and propose uplifts the overall level of security in an organisation.</p>

Project Objective
-----------------
`What type of hashing algorithm was used to protect passwords?`

<p>Some common hashing algorithms include MD5, SHA-1, SHA-2, NTLM, and LANMAN.</p><br>

`What level of protection does the mechanism offer for passwords?`

<p>This cryptographic hash function takes user input — the password — and turns it into a seemingly 
random sequence of numbers. There are only two ways to crack a good cryptographic hash function. 
One of them is the infamous brute-force attack, when a hacker simply tries all possible combinations
of the password until he’s able to find a match.</p><br>

`What controls could be implemented to make cracking much harder for the hacker in the event of a password database leaking again?`

<p>Salting:<br>
A salt randomizes each hash by adding random data that is unique to each user to their password hash,
so even the same password has a unique hash. If someone tried to compare hashes in a rainbow table to
those in a database, none of the hashes would match, even if the passwords were the same.</p><br>

`What can you tell about the organization’s password policy (e.g. password length, key space, etc.)?` <br>
  - Password should be of length more than 7.<br>
  - Characters, small letters, numbers and capital letters must be included in password.<br>
  - Unnecessary details must not be mandatory to be filled.<br>
  - Don’t let users include their username, actual name, date of birth and other personal information while creating a password.<br>
  
`What would you change in the password policy to make breaking the passwords harder?`
  - Reliable hashing functions like <mark>SHA-256</mark> and <mark>bcrypt</mark> are recommended and 
    common hashing function like MD5 should not be used.<br>
  - Salting should be used. <br>
  - Investing in encryption software, it is foolproof way to safeguard your database and ensure that
    anyone trying to hack in is unable to read the information presented in the database.<br>
<br>


**By analysing all the passwords which are leaked:**<br>

![Datasheet of leaked password](./datasheet(1).png)<br>
![Datasheet2 of leaked password](./datasheet(2).png)

```
I have noticed that all the leaked passwords are of length less than 7 
and passwords with no characters are easier to crack. There are so
many websites which can change any plaintext to MD5 hash, so, always 
stay away from making common passwords. 
Hackers use high quality of graphics card in their system, because they 
will try to compare a massive quantity of strings to your hash, and 
the one that validates is very likely your password. With weak password
hashing algorithms, what hackers will do is try millions, or billions 
of different combinations - as fast as their hardware allows.
bcrypt is computationally slow, so this cracking will be slowed down
immensely. Bcrypt can help slow cracking down to the point where youcan 
only do a few tests per second, if that. This is due to the computational cost factor.
```

Resources
---------
[To read more about Bcrypt](https://security.stackexchange.com/questions/61385/the-brute-force-resistence-of-bcrypt-versus-md5-for-password-hashing/61387#61387)<br>
[Password attack types and how to prevent them](https://threatmodeler.com/top-5-password-attack-types-and-how-to-prevent-them/)<br>
[Convertor of MD5 hash to plaintext](https://md5decrypt.net/en/)<br>
[To read more about SHA-256 and convertor of plaintext to SHA-256 hash](https://www.movable-type.co.uk/scripts/sha256.html)<br>
