# hooks-for-gitinfo2

To make the set up of gitinfo2 more pleasant (at least for myself!). Modified to allow *any* tags to be identified as release tags (see the "Tailoring release tags" section in the [gitinfo2](http://mirrors.ibiblio.org/CTAN/macros/latex/contrib/gitinfo2/gitinfo2.pdf>) package documentation):

1. Put `post-checkout`, `post-commit` and `post-merge` under `.git/hooks`,
2. Run `git checkout master` in your git repository's root directory.
3. Hopefully it will work. If you are warned that `post-checkout` is not executable, then make it so (as well as `post-merge` and `post-commit`!). For mac users, see [this](https://support.apple.com/guide/terminal/make-a-file-executable-apdd100908f-06b3-4e63-8a87-32e71241bab4/mac).

For how to tag, see [this](https://git-scm.com/book/en/v2/Git-Basics-Tagging).