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


# Flag1
## Steps
1. Once logged in as 'user', visit 'My Profile' tab
2. Look at url of tab (i.e. https://XXXXXXXXXXXXXXXXXXX.ctf.hacker101.com/index.php?page=profile.php&id=c)  ('XXXXXXXXXXXXXXXXX' is arbitrary)
3. Change 'index.php?page=profile.php&id=c' to 'index.php?page=profile.php&id=b' in url 
 
## Thought Process
My thought process behind this was to search around the 'user' profile to see if I could find another flag. Once I saw the url on the 'My Profile' tab, my first thought was to see if I could visit other pages and ids in the url. Upon seeing that I was getting valid pages to return, I knew that I could do a path traversal. I tried 'id=a' at first. No luck. Then I tried 'id=b'. BOOM! Flag











# Tools Used
