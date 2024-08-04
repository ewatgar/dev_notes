# Index
1. [Config SSH key for GitHub on WSL2](#config-ssh-key-for-github-on-wsl2)

## Config SSH key for GitHub on WSL2
### Steps
1. Git config

    ```
    git config --global user.name "username"

    git config --global user.email "github_email"
    ```
2. Create ssh key

    ```
    ssh-keygen -t ed25519 -C "github_email"
    ``` 
    For other name, write as `/home/user/.ssh/key_name`

3. Copy .pub key (public key) and paste on GitHub profile
    ```
    cat ~/.ssh/key_name.pub
    ```
4. Clone any repo from GitHub


### Video (spanish)
https://www.youtube.com/watch?v=o_jn9KSxFuc