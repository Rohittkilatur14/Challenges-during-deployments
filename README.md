First Challenge : 

Ansible download issue in thor server:

Package Manager was not installed properly so had to face deprecacies relating to Ansible download, so later had to run certain commands and then with right package manager version, I was able to run it successfully and download it correctly as previous versions were downgraded versions and not compatible with the current production server configurations


Second Challenge :

Mariadb starting issues in Production servers:

Happened due to corrupted conf files while downloading Mariadb and adding it to the right file path, so changed the ownership of the main configuration file of mysql which is package manager for MariaDb to '-R' and then it worked fine.....


Third Challenge :

SSH passwordless login issue as the paraphrase : 

Paraphrase kept appearing even after logging into production servers due to private keys not getting accessed by ssh-agents, so had to ensure that public keys were running the right private keys at the backend using process ids, which would enable session for 'no-paraphrase' to be entered and login to ssh-production servers would become very easy again.


