

Git bisect exercise
===================

The script calculates pi using the 100 first terms of the Nilakantha series.
At each commit, the 100 terms are reshuffled.
At some point within the 1000 first commits, an error was introduced.

Use `git bisect` to find the commit which broke the computation.

Bonus: write a script that checks for a correct result and use
`git bisect run` to find the offending commit automatically.
