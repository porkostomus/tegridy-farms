# tegridy-farms

HTTP Integration with GitHub and Twitter

Write a program that will poll a GitHub repo, look for new pull requests, and tweet a summary of each PR to Twitter.

Some practical considerations:

A dummy github repo should be created and API access be enabled
A dummy twitter account should be created and API access should be enabled
Getting the PRs via webhook might be impractical (especially considering that we should be able to easily run and test your program). Suggestion: the program can start up, gather the latest PR's, post them to Twitter, then exit. Subsequent runs of the program should pick up PR's that have come in since the last time. (How will you persist the state between runs?) .... Alternately, the program can run forever and periodically poll the GitHub repo for changes.

Constraints

Make plain HTTP requests against GitHub and Twitter, i.e., do not use a 3rd party Github or Twitter SDK.
