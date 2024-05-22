# SSH Key Creation

```
ssh-keygen -t rsa -b 4096 -C "<your email address>"
cd ~/.ssh
ls
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa

```
# Add SSH to Repo 

```
cat ~/.ssh/id_rsa.pub (or clip)
```
(SSH and GPG keys )

