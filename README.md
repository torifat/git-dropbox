git-dropbox
======

a dropbox wrapper for git

##Installation

```bash
$ curl -skL http://git.io/git-dropbox > /usr/local/bin/git-dropbox
$ chmod +x /usr/local/bin/git-dropbox
```

##Usage

First you have to set your Dropbox Git repository path -

```bash
$ git config --global dropbox.path <path>
```

For example I have my dropbox installed in `~/Dropbox`. So, I've created a folder called `Git` in there and then run the following command in my terminal -

```bash
$ git config --global dropbox.path ~/Dropbox/Git
```

Now, to enable dropbox support for any git repository, do the following -

```bash
$ git dropbox init
```

Now, to push your changes to dropbox -

```bash
$ git dropbox push
```

If you run `git dropbox` for at least once. Then, It'll create an alias `db` for you. So, you can do `git db <command>` instead of `git dropbox <command>` after the first run.  