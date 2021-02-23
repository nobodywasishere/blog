# blog

A simple command-line blog manager for Jekyll written in Python.

Inspired by https://github.com/automoto/devlog.

Tested against Python 3.9 on Arch Linux.

Requires argparse, [bat](https://github.com/sharkdp/bat), and [simple-term-menu](https://github.com/IngoMeyer441/simple-term-menu)

Set env variable `BLOG_DIR` to your Jekyll blog website. Uses the default `_drafts` for draft posts and `_posts` for posts. Automatically commits changes once done editing a post. Drafts must end with `.md`.

```
usage: blog [-h] [-p] [--blog_folder BLOG_FOLDER] [--editor EDITOR] [-l] [-d] [-f FIND] [-s] [--push]
            [--version]
            [post_title]

positional arguments:
  post_title            Name of the blog post (without date or file ext)

optional arguments:
  -h, --help            show this help message and exit
  -p, --post            Post a draft (copy to _posts with date, git add/commit)
  --blog_folder BLOG_FOLDER
                        Location of blog folder (overrides env variable)
  --editor EDITOR       Editor to open posts with (overrides env variable)
  -l, --list            List all current drafts
  -d, --delete          Delete a draft
  -f FIND, --find FIND  Search within drafts
  -s, --serve           Serve the blog website with drafts
  --push                git push when committing changes
  --version             show program's version number and exit
```
