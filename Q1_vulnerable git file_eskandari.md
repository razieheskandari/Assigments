
# Question1: 
Many websites expose their “.git” files, please show how it could be dangerous.
# The Answer:

If a website exposes their gif files, even if directory listing was disabled, the attacker could still utilize some tools to get all part of remote repository on his computer. One example of such tools is GitTools.
Then, the following commands (GitTools/gitdumper.sh) could be used by the attacker to checkout (download) the whole websites’ repository:
`./gitdumper.sh websitename/.git/ /output-directory/`

`git status 		`

`git checkout --  	`

`git log	    	`

Hackers get just enough information to hack into the website!! Since the attacker has now a full access to the source code of the website! 

He could analyze the source code to find vulnerabilities. It needs mentioning that source code is everything! This kind of analysis (Static Analysis) along with the ability to execute the site at the same time (Dynamic Analysis) is the most powerful analysis, results in finding much vulnerability in the website. 

Even more, the attacker may obtain some credentials, authentication tokens, etc in some sensitive files of the repository.

For more information, please see the following link:

[source code disclosure via git file](https://pentester.land/tutorials/2018/10/25/source-code-disclosure-via-exposed-git-folder.html)


## Running an Example:
1- we first should find some .git exposure on the web, by running one of the following methods:  
	
	a-use google hacking tricks:  
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q1(1).png)
	
	b-use the following command to scan for git exposure:  
`	nmap --open -PN -n -p80,81,82,8000,8080,443,8443,9443 --script http-git -oA http-git -iL domains.lst`

2-Then, here we select this site (https://codemirror.net/) as an example vulnerable one. 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q1(2).png)

3- now, we need a script to automate downloading of site's content. GitHack.py [from this link ](https://github.com/lijiejie/GitHack), could handle this job well.

4- run  GitHack.py on the beforementioned exploitable site

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q1(3).png)

5-the result is having a local mirror of site which gives attackers the ability to access to the whole site content, as well as its source code!

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q1(4).png)

