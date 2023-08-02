
# Development

Clone the repository
```
git clone https://github.com/cardenca/LumpenVille.git
```
If you clone by http in each push the prompt will ask you for your github credentials. If you have your ssh key configure, you can clone using ssh:
```
git clone git@github.com:cardenca/LumpenVille.git
```

Create a new branch from main
```
git checkout -b name_branch
```

Do stuff
You can see how the page is looking with 
```
mkdocs serve
```

Commit the changes you want to include, the push the changes to the remote github
```
git add .
git commit -m 'message to understand what the commit include'
git push --set-upstream origin name_branch
```

To see the changes you made, you can use
```
git diff
git status
```

When you want to publish the page you need to make a pull request from the new branch to main. When it is merge the page will update automatically.

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
