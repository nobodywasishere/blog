# blog

A simple command-line blog manager for Jekyll written in Python

Tested against Python 3.9 on Arch Linux

```
usage: blog [-h] [-p] [--blog_folder BLOG_FOLDER] [--editor EDITOR] [-l] [-s] [-d] [post_title]

positional arguments:
  post_title            Name of the blog post (without date or file ext) (required if not passing -l)

optional arguments:
  -h, --help            show this help message and exit
  -p, --post            Post a draft (copy to _posts with date, git add/commit/push)
  --blog_folder BLOG_FOLDER
                        Location of blog folder (overrides env variable)
  --editor EDITOR       Editor to open posts with (overrides env variable)
  -l, --list            List all current drafts
  -s, --serve           Serve the blog website with drafts
  -d, --delete          Delete a draft
```
