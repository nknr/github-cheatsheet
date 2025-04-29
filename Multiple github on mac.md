
**Step 1: Generate SSH keys for each account**

```
# Personal account
ssh-keygen -t rsa -C "your_personal_email@example.com" -f ~/.ssh/id_rsa_personal

# Work account
ssh-keygen -t rsa -C "your_work_email@company.com" -f ~/.ssh/id_rsa_work
```

**Step 2: Add SSH keys to the agent**

```
ssh-add ~/.ssh/id_rsa_personal
ssh-add ~/.ssh/id_rsa_work
```
**Setp 3: Using echo (for small additions)**

```
echo -e "\nHost github-personal\n\tHostName github.com\n\tUser git\n\tIdentityFile ~/.ssh/id_rsa_personal" >> ~/.ssh/config

echo -e "\nHost github-work\n\tHostName github.com\n\tUser git\n\tIdentityFile ~/.ssh/id_rsa_work" >> ~/.ssh/config
```

**Setp 3: Using cat with here-document (easier for multiple lines)**

```
cat <<EOL >> ~/.ssh/config

# Personal GitHub
Host github-personal
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa_personal

# Work GitHub
Host github-work
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa_work
EOL
```

**Step 4: View contents manually**
```
cat ~/.ssh/id_rsa_work.pub
```

Copy and paste that into GitHub > Settings > SSH and GPG keys.

**Step 4: Verify**
```
ssh -T git@github-work
```
