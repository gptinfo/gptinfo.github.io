```bash
rm -rf .git
git init
git config --local user.name "admin"
git config --local user.email "admin"
git add .
git commit -m "first commit"


git remote remove origin
git remote add origin git@github.com:gptinfo/app.git
git push -u origin main
```

```
https://gptinfo.github.io/app/privacy.html
```

```
ssh-keygen -t ed25519 -C "admin@gmail.com" -f ~/.ssh/id_ed25519


Host github-gptinfo
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_ed25519

git remote set-url origin git@github-gptinfo:gptinfo/gptinfo.github.io.git
git config user.name "admin"
git config user.email "admin@gmail.com"
cat ~/.ssh/id_ed25519.pub
ssh -T git@github-gptinfo
```