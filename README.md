# Orbs Assignment
## Documentation
### Create Repo
First, I created a new repo in Github and cloned my code from the calculator assignment over. That would form the base of my assignment.
### Link to CircleCI
Next, I linked the repo to CircleCi and began running some tests. This took a few commits to get into what I believed would be a working state.
### Configure Slack Orb
I included a reference to the Slack orb at the beginning of my CircleCI config file and I created a context in the CircleCI web UI with two environmental variables to be passed to the orb. The two defined variables were for the authentication token and the default channel to send to. I also included a code snipet showing how you might format a message block from the Slack orb from some documentation I read on the orb. The orb appears to check for a successful build then tries to send a message as intended.
### Problems
I was unable to get my code to send a message to the Slack channel. I kept getting an error about an incorrect Slack key format. This is the best I could accomplish with the time I spent on it.