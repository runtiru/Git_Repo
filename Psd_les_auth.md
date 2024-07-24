# How to setup password less authentication for private git repository to local machine..?

- Create a private git repositioty + add a readme file
  - clone this repository on your local use `HTTPS` (gitbash)

```sh
git clone https://github.com/your_username/your_repo.git 
    `or`
git clone -b main https://github.com/your_username/your_repo.git
`-b main` used for defalut branch is main
```

- open github settings --> `ssh and gpg keys`
  - SSH key
    - Check out our guide to `connecting to GitHub using SSH keys` or troubleshoot `common SSH problems`.
      - open `connecting to GitHub using SSH keys`
        - open `Generating a new SSH key and adding it to the ssh-agent`
    - chek your machine windows or mac or linux

- in windows
  - copy the Generating a new SSH key command and change your mail what you give your github account..
  - Open gitbash (always)

```sh
ssh-keygen -t ed25519 -C "tirumalagadiya@gmail.com"
> enter -> generate public and private key
> enter -> enter file in which to sava the key
> enter passphrase (not recommended)
```

check the public key & copy the public key

```sh
cat /user/balu/.ssh/id_ed25519.pub
```

Now goto github account:

- open github settings --> `ssh and gpg keys`
  - SSH keys
  - create new ssh key
  - give a title (ex: windows ssh)
    - paste the public key on the key section

- Add SSH Key

* Now tesh the ssh key:
  - open github settings --> `ssh and gpg keys`
  - open `connecting to GitHub using SSH keys`
  - Testing your SSH connection
  - check windows user open gitbash 
  - copy the command and paste on gitbash

```sh
ssh -T git@github.com
```

- enter the passphrase (if you give the passphrase)
  - if you get the message `Hi tirumalagadiya! You've successfully authenticated.

- you should give first attemt to username and password

```sh
git push
Username - tirumalagadiya@gmail.com
Password - ******
```

* Git commands:-

- git init
- git add .
- git commit -m "message"
- git push

* Git add and commit in a same repository..?

- git commit -am "message"

- git push -u origin master
- git remote add origin https://github.com/tirumalagadiya/firstrepo.git
- git pull
- git clone
- git status
- git log
- git branch
- git checkout
- git merge
- git diff
- git reset
- git revert
- git stash
- git tag
- git remote
- git fetch
- git push
- git config
- git help
- git remote -v
- git remote add origin https://github.com/tirumalagadiya/firstrepo.git
- git remote set-url origin https://github.com/tirumalagadiya/firstrepo


# how to change git private repository to public repository..?