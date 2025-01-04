Name = Rajdeep Naskar
Company = CODTECH IT SOLUTIONS
ID = CT6WDS2467
Domain = CYBER SECURITY AND ETHICAL HACKING
Duration = November to 10th january 2025
Topic = password strength checker

OVERVIEW OF THE PROJECT:

In this program, we will be taking a password as a combination of alphanumeric characters along with special characters, and checking whether the password is valid or not with the help of a few conditions.

Primary conditions for password validation:

Minimum 8 characters.
1. The alphabet must be between [a-z]
2. At least one alphabet should be of Upper Case [A-Z]
3. At least 1 number or digit between [0-9].
4. At least 1 character from [ _ or @ or $ ].

l, u, p, d = 0, 0, 0, 0
s = "rA@j$d_deep02"
if (len(s) >= 8):
    for i in s:

        # counting lowercase alphabets 
        if (i.islower()):
            l+=1            

        # counting uppercase alphabets
        if (i.isupper()):
            u+=1            

        # counting digits
        if (i.isdigit()):
            d+=1            

        # counting the mentioned special characters
        if(i=='@'or i=='$' or i=='_'):
            p+=1           
if (l>=1 and u>=1 and p>=1 and d>=1 and l+p+u+d==len(s)):
    print("Valid Password")
else:
    print("Invalid Password")
