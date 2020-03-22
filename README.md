# opencontribution

# Introduction

SSH, or secure shell, is an encrypted protocol used to administer and communicate with servers. When working with an Ubuntu server, chances are you will spend most of your time in a terminal session connected to your server through SSH.

In this guide, we’ll focus on setting up SSH keys for a vanilla Ubuntu 16.04 installation. SSH keys provide an easy, secure way of logging into your server and are recommended for all users.

# Step 1 — Create the RSA Key Pair

The first step is to create a key pair on the client machine (usually your computer):

Linux command: ssh-keygen

# Step 2 — Copy the Public Key to Ubuntu Server

The quickest way to copy your public key to the Ubuntu host is to use a utility called ssh-copy-id. Due to its simplicity, this method is highly recommended if available. If you do not have ssh-copy-id available to you on your client machine, you may use one of the two alternate methods provided in this section (copying via password-based SSH, or manually copying the key).

# Copying Public Key Manually

If you do not have password-based SSH access to your server available, you will have to complete the above process manually.

We will manually append the content of your id_rsa.pub file to the ~/.ssh/authorized_keys file on your remote machine.

To display the content of your id_rsa.pub key, type this into your local computer:

Linux Command: sudo nano ~/.ssh/id_rsa.pub

# SSH setup command for first time
sudo ssh -T surendra246@github.com

# Create clone with all existing folder and files
git clone git@github.com:surendra246/restapi.git

git remote -v


# create a new repository on the command line

echo "# opencontribution" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:surendra246/opencontribution.git
git push -u origin master
                

# push an existing repository from the command line

git remote add origin git@github.com:surendra246/opencontribution.git
git push -u origin master
