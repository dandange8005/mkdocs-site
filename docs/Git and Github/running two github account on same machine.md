Today I would like to share with you how to run two github account on the same machine.

I have two github accounts, one for personal and one for testing. I would like to keep them separate so that I can run some tests using the two accounts to test the collaboration workflow.

I looked up some tutorials on how to do this and I am going to go ahead and try it out.

- [Using multiple github accounts on same machine](https://www.youtube.com/watch?v=vSeYsk4WYvg&ab_channel=SciTechEnthusiasts)
- [Generate git ssh keys for multiple git accounts in one machine | Mac setup](https://youtu.be/iWr9m9IH5xI)

Basica steps:

- Create ssh keys for each github account
- Git config file
- Add ssh keys to Github account
- Test the ssh keys





## Step 1: Create a new ssh key

The first step is to create a new ssh key for the new github account.

```bash
ssh-keygen -t rsa -C "firstaccount@email.com"
```

You will be prompted to enter a file name for the ssh key. I would recommend using the default file name `id_rsa` and `id_rsa.pub`.

You will also be prompted to enter a passphrase for the ssh key. You can leave it blank if you don't want to enter a passphrase.

## Step 2: Add the new ssh key to the ssh-agent

The next step is to add the new ssh key to the ssh-agent.

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

## Step 3: Add the new ssh key to the github account

The next step is to add the new ssh key to the github account.

You can copy the contents of the public key `id_rsa.pub` and paste it into the github account settings.

## Step 4: Create a new ssh config file

The next step is to create a new ssh config file.

```bash
touch ~/.ssh/config
```

You can then add the following lines to the config file.

```bash
# Personal account, this is the default account
Host github.com
   HostName github.com
   User git
   IdentityFile ~/.ssh/id_rsa

# Work account
Host github-work
   HostName github.com
   User git
   IdentityFile ~/.ssh/id_rsa_work
```

## Step 5: Clone the repo using the new ssh config

The next step is to clone the repo using the new ssh config.

```bash
git clone git@github-work:username/repo.git
```

## Step 6: Add the new ssh config to the ssh-agent

The next step is to add the new ssh config to the ssh-agent.

```bash
ssh-add ~/.ssh/id_rsa_work
```

## Step 7: Test the new ssh config

The next step is to test the new ssh config.

```bash
ssh -T git@github-work
```

You should see the following message.

```bash
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

## Step 8: Add the new ssh config to the git config

The next step is to add the new ssh config to the git config.

```bash

git config --local user.name "username"
git config --local user.email "
```

## Step 9: Test the new git config

The next step is to test the new git config.

```bash
git config --list
```

You should see the following message.

```bash
user.name=username
user.email=
```

## Step 10: Push the changes to the new github account

The next step is to push the changes to the new github account.

```bash
git push origin master
```

## Step 11: Test the new github account

The next step is to test the new github account.

```bash
ssh -T git@github-work
```

You should see the following message.

```bash
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

## Step 12: Add the new ssh config to the ssh-agent

The next step is to add the new ssh config to the ssh-agent.

```bash
ssh-add ~/.ssh/id_rsa_work
```
