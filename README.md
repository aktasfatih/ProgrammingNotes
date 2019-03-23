## Github
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - It is the best fource for learning Markdown syntax that Github uses.
- I use a plugin on VSCode to preview my Markdown files.


## Docker
- [Building Efficient Dockerfiles](http://bitjudo.com/blog/2014/03/13/building-efficient-dockerfiles-node-dot-js/) - Website explaining why to not rebuild node apps.

Snippet for using ```package.json```,
```
ADD package.json /tmp/package.json
RUN cd /tmp && npm install
RUN mkdir -p /opt/app && cp -a /tmp/node_modules /opt/app/
```



