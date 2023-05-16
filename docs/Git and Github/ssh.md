# SSH

This is me trying to set up SSH on my MacBook pro 13". I am following the tutorial on Github.

The tutorial I followed:

- [Generating a new SSH key and adding it to the ssh-agent - GitHub Docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
- [Setting Up SSH Keys for GitHub - YouTube](https://www.youtube.com/watch?v=8X4u9sca3Io&t=2s&ab_channel=VictorGeislinger)

## Checking for existing SSH keys

To check if there are any existing keys

```
$ ls -al ~/.ssh
```

## Generating a new SSH key and adding it to the ssh-agent

1. Generate my first ssh key on my MacBook pro 13"

    `$ ssh-keygen -t ed25519 -C "nelson_zhang80@hotmail.com"`

2. Enter file in which to save the key `'/Users/nanzhang/.ssh'.`
   
3. Enter a pass: `La************`
  
    ```
    Your identification has been saved in /Users/nanzhang/.ssh/id_ed25519
    ```
  
4. Public key generated
  
    ```
    Your public key has been saved in /Users/nanzhang/.ssh/id_ed25519.pub
    The key fingerprint is:
    SHA256:ahbJom8JMCNsce0vB5eM1SJ1jgFx30YuN0E5zWXBaLg nelson_zhang80@hotmail.com
    The key's randomart image is:
    +--[ED25519 256]--+
    |    .o++...+= ++.|
    | . . o.o*.++.=.. |
    |. o . =.o+ *+    |
    |=o   = =  +E.    |
    |o+  . B S        |
    |  .. o =         |
    |  .. .*          |
    |   .oo           |
    |   ..            |
    +----[SHA256]-----+
    ```
  
5. To show the public key
  
    ```
    $ cat ~/.ssh/id_ed25519.pub
    ```
  

## Adding the newly generated key to the ssh-agent

The ssh-agent is like a wallet that keeps all the keys in place

command:

1. Start the ssh-agent in the background.

    ```
    $ eval "$(ssh-agent -s)"

    Agent pid 28926
    ```

2.  Open your `~/.ssh/config` file, and type in
  
    ```
    Host github.com
    AddKeysToAgent yes
    UseKeychain yes
    IdentityFile ~/.ssh/id_ed25519
    ```
  
3. Then add this command
  
    ```
    ssh-add --apple-use-keychain ~/.ssh/id_ed25519
    ```

## Adding the public key to Github

1. print the key in terminal
  
    ```
    cat ~/.ssh/id_ed25519.pub
    ```
  
2. copy the key  
3. go to Github and add the key to settings