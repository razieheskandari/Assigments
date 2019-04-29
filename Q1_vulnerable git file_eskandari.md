
# Question1: 
Many websites expose their “.git” files, please show how it could be dangerous.
# The Answer:

If a website exposes their gif files, even if directory listing was disabled, the attacker could still utilize some tools to get all part of remote repository on his computer. One example of such tools is GitTools.
Then, the following commands (GitTools/gitdumper.sh) could be used by the attacker to checkout (download) the whole websites’ repository:
`./gitdumper.sh websitename/.git/ /output-directory/`

`git status 		`

`git checkout --  	`

`git log		`

Hackers get just enough information to hack into the website!! Since the attacker has now a full access to the source code of the website! 

He could analyze the source code to find vulnerabilities. It needs mentioning that source code is everything! This kind of analysis (Static Analysis) along with the ability to execute the site at the same time (Dynamic Analysis) is the most powerful analysis, results in finding much vulnerability in the website. 

Even more, the attacker may obtain some credentials, authentication tokens, etc in some sensitive files of the repository.

For more information, please see the following link:

[source code disclosure via git file](https://pentester.land/tutorials/2018/10/25/source-code-disclosure-via-exposed-git-folder.html)



