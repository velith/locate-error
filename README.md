

Git bisect exercise
===================

The script `get_pi.py` calculates pi using the 100 first terms of the
Nilakantha series.  It should produce 3.141592 but it does not. It produces
3.264592 using the last commit.  At each commit, the 100 terms are reshuffled.
At some point within the 1000 first commits, an error was introduced. The only
thing we know is that the first commit worked correctly.

Use `git bisect` to find the commit which broke the computation.

Bonus: write a script that checks for a correct result and use `git bisect run`
to find the offending commit automatically.

The motivation for this exercise is to be able to do archaeology with Git on a
source code where the bug is difficult to see visually. Finding the offending
commit is often more than half the debugging.  In this particular example the
knowledge about the offending commit will not help us but in reality mastering
git bisect is a huge time saver.
