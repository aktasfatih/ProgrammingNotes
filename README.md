## Github
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - It is the best fource for learning Markdown syntax that Github uses.
- [Github Formatting](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#quoting-code) - Official Docs for Markdown

**NOTES**:
- I use a plugin on VSCode to preview my Markdown files.


## Docker
- [Building Efficient Dockerfiles](http://bitjudo.com/blog/2014/03/13/building-efficient-dockerfiles-node-dot-js/) - Website explaining why to not rebuild node apps.

Snippet for using ```package.json```,
```
ADD package.json /tmp/package.json
RUN cd /tmp && npm install
RUN mkdir -p /opt/app && cp -a /tmp/node_modules /opt/app/
```

#### Instructions to remember

###### NODEJS AND DOCKER
```
FROM image:version # Image to build from
WORKDIR # Creating an app directory
COPY
```


## NodeJS
- [Intro for NodeJS with Docker](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/) - Making a simple Express app for Docker containers

## Linux Notes
```
touch [FILE] # Creates an empty file named FILE

```

