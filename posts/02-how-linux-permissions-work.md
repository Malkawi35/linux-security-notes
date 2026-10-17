# How Linux permissions work

In one of the Bandit labs, I had to `cat` a file owned by bandit1, but it said permission denied — because a different user without the right permissions can't access it. Running `ls -l` showed me why: only the owner could read it, and I (like everyone else) could not. I even tried `sudo`, but that didn't work either.

What I understood from all those tries is that Linux decides access by who you are, not how hard you push. The issue was my identity.
