[[6  - Introduction of SSH Key Types]]

- Before adding a new SSH key to the ssh-agent to manage your keys, you should have checked for existing SSH keys and generated a new SSH key.

1. Start the ssh-agent in the background.

> $ eval "$(ssh-agent -s)"

![[ssh-agent.png]]

2. Add your SSH private key to the ssh-agent.

> ssh-add ~/.ssh/id_ed25519


![[ssh-add.png]]

