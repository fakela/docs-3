
# PeeringDB Documentation

As viewable at http://docs.peeringdb.com/

*NOTE* Please do not put issues here anymore, new issues should be created at <https://github.com/peeringdb/peeringdb/issues>

### Modifying these docs

To work on and change these documents, you'll need git, python, and pip.

- CentOS
    ```
    sudo yum install python-pip
    ```

Install [MkDocs](http://www.mkdocs.org/)
```sh
pip install mkdocs
```

Fork the repo
- click the fork button on <https://github.com/peeringdb/docs>
- select your github username

Clone the repo
```sh
git clone git@github.com:$GITHUB_USERNAME/docs.git
cd docs
```

Start mkdocs
```sh
mkdocs serve
```

or, if you'd like to specify the port, use -a $ADDRESS:$PORT, for example:

```sh
mkdocs serve -a 0.0.0.0:7889
```

You should now see a message similar to:
    Serving on <http://127.0.0.1:8000>

Point your browser at that URL, and you'll get real time updates to the generated documentation as you edit.

Markdown has its own formatting syntax, to get started look [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for an excellent cheatsheet.

### Updating the site

Once you are happy with your changes, commit and push, then run

```sh
mkdocs gh-deploy
```

After that, you will be able to view your changes at `$GITHUB_USER.github.io/docs`.