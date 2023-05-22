# Postbook Solution Write-up


Difficulty: Easy

Type: Web Exploitation

Flags: 7 

-----------------------------------------
# Flag0 
## Steps
1. Visit https://XXXXXXXXXXXXXXXXX.ctf.hacker101.com/index.php ('XXXXXXXXXXXXXXXXX' is arbitrary)
2. Make an account. Search around website to familiarize 
3. Notice 'user' profile. Attempt to sign in to 'user' with a weak password

## Thought Process
My thought process behind finding the first flag was to use random passwords to brute force into account. After trying 'user', 'pass', and 'password' as passwords 
you'll see that providing 'password' grants you access into the account. The flag is then displayed on screen. I imagine that a password cracker could have been useful 
for this if the password was any more secure.










# Tools Used
