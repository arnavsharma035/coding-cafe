#CODING CAFE

###Q1: What did pwd print?
    It shows the absolute path of the file.

###Q2: What did ls -a show that plain ls did not?
    ls -a showed the hidden files like the ones starting with a dot, as plain ls hides anything that starts with a dot by default.

###Q3: Pick one line from ls -l. What do you think the first column means?
    the first column is a string like -rw-r--r--, and it shows the file type and permissions. The first character tells you if it's a file (-)  or a directory(d).

###Q4: Why does that work from where you are standing? Which kind of path is coding-cafe/week02?
Absolute or Relative?
    It works because I'm giving the shell a path starting from where I currently am, so it's a relative path. It doesn't start with /, so it's not absolute, it just tells ls to look inside the coding-cafe folder for week02 without me having to move there first.

###Q5: mv did two different jobs above. What were they?
    First it moved the file into a different folder (week01/) without changing its name. Then it renamed the file in place, from README-backup.md to old-rename.md, without moving it anythere. So mv is really both "move" and "rename" depending on what you give it.

###Q6: How many folders are on your PATH?
    Mine has 21 folders separated by colons.

###Q7: Write down exactly where your python3 lives.
    /usr/bin/python3

###Q8: Compare your answer to 6 with the person next to you. Are they the same? If not, why might that be?
    Ours were different as my was 21 and my friend's was 27 and this might be because one of us installed Python through a different method.

###Q9: What exactly did the shell say? Explain the error in your own words, using the word PATH.
    The shell said pyton3: command not found. That's because the shell only looks through the folders listed in PATH for a matching program name, and since "pyton3" is misspelled, no folder on PATH has anything by that name.

###Q10: .venv did not appear with plain ls. Why not?
    Because .venv starts with a dot, which makes it a hidden file/folder by convention. I had to use ls -a to see it, same as question 2.

###Q11: What changed about your prompt?
    (.venv)appeared at the very start of my prompt, before my username. It's the shell's way of showing me I'm currently inside that virtual environment. 

###Q12: Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell
you about what activate actually did to your PATH?
    No, this time which python3 pointed inside the .venv folder instead of /usr/bin/python3. That tells me activate didn't install a new Python - it just changed my PATH so the venv's copy gets found first.

###Q13: What is in the second list that was not in the first?
    The second list had requests in it (plus its dependencies like charset-normalizer and idna). The first was basically empty or just had itself.

###Q14: Where does python3 point now?
    Back to /usr/bin/python3, same as before I activated the venv. deactivate just restores my PATH to what it was.

###15: Find what ls -h does. Write it in your own words
    It shows file sizes in human- readable form, like 4.0K or 1.2M instead of raw byte counts. Way easier to read at a glance.

###16: What is the difference between what Ctrl + C and Ctrl + D did?
    Ctrl+C interrupted the running Python process and kicked me back to the >>> prompt without closing it. Ctrl+D actually exited the Python interpreter completely, sending an "end of input" signal instead of an interrupt.