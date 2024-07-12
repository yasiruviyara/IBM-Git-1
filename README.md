# SSH Key Creation

```
ssh-keygen -t rsa -b 4096 -C "<your email address>" [ optinal check  >> cd ~/.ssh && ls after come main derc]

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa

```
# Add SSH to Repo 

```
cat ~/.ssh/id_rsa.pub (or clip)
```

```
clip < C:\Users\User/.ssh/id_rsa.pub.
```
(SSH and GPG keys )

