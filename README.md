# GitEasy-Bash
A package of short bash scripts to automate git synchronisation.

## How to install?
- Clone or [download zip](https://github.com/avirukbasak/GitEasy-Bash/archive/main.zip) and extract.
- Open up a terminal in that directory.
- Execute `install.sh` (or `termux-install.sh`).
- Note that root permission is needed to install (except termux).
- Or you can manually copy the files to `/usr/bin`.

## In this pack
- The pack contains 3 commands
- In `gauth`, you enter your Git `username`and `email`. The values are stored in `~/.gitauto` as an `ssh` URL. It's for one time use.
- `gauth` also adds `git global config for user and email`.
- `ginit` initialises the repository and adds or edits a remote named `origin`. 
- Before cloning you must execute `ssh-keygen` when suggested by `gauth`.
- Then you must add the public key to [GitHub keys settings](https://github.com/settings/keys).
- `gclone` clones from account entered in `gauth`.

## How to use?
- Use `gauth` once after installation to write the string `ssh://git@githib.com/user` in `~/.gitauto`
- Run `ssh-keygen` when asked by `gauth`.
- Copy the public key from the file and add it to you account.
- Clone `your` repository.
- Change to that directory.
- Once pulled and ready you can make changes.
- Once your work is done, use `git push`.
- Set up upstreap if asked.
