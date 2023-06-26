# Github 

## add new ssh key:
* ### (Linux)
	`ssh-keygen -t ed25519 -C "willocoro25@gmail.com"`
	add the key to the ssh agent:
	`eval "$(ssh-agent -s)"`
	copy the generated key that will be something like...
	`cat ~/.ssh/id_ed25519.pub`
	now go to (https://github.com/settings/keys) and click on new ssh key,
	now you can clone your projects