## Github
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - It is the best fource for learning Markdown syntax that Github uses.
- [Github Formatting](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#quoting-code) - Official Docs for Github's formatting.

**NOTES**:
- I use a plugin on VSCode to preview my Markdown files.


## Docker
- [Building Efficient Dockerfiles](http://bitjudo.com/blog/2014/03/13/building-efficient-dockerfiles-node-dot-js/) - Website explaining why to not rebuild node apps.
- [Deploy Docker Containers](https://aws.amazon.com/getting-started/tutorials/deploy-docker-containers/) - ECS to run containers
- [Dockerizing a NodeJS Application](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/) - Setting up a simple nodejs app in a container

**NOTES**:
```
docker build -t <your username>/node-web-app . #  The -t flag lets you tag your image so it's easier to find later using the docker images command
docker images # Seeing images
```

###### CODE SNIPPETS
Using ```package.json``` in Docker,
```
ADD package.json /tmp/package.json
RUN cd /tmp && npm install
RUN mkdir -p /opt/app && cp -a /tmp/node_modules /opt/app/
```

Example for ```dockerfile```,
```
FROM image:version # Image to build from
WORKDIR # Creating an app directory
COPY package*.json ./ # Copying package and lock file if exists.
RUN npm install # Installing dependencies
RUN npm ci --only=production # For production
```

## NodeJS
- [Intro for NodeJS with Docker](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/) - Making a simple Express app for Docker containers
- [Installing Node on Ubuntu](https://websiteforstudents.com/install-the-latest-node-js-and-nmp-packages-on-ubuntu-16-04-18-04-lts/) - Well..
- [Facebook login](https://codeburst.io/node-js-rest-api-facebook-login-121114ee04d8?gi=d9ee6ee0b1d)
- [Social OAuth](https://alexanderpaterson.com/posts/add-social-authentication-to-a-react-native-application) - NodeJS Express OAuth integration, requires xcode
- [Login with FacebookSDK](https://developers.facebook.com/docs/react-native/login/) - Others require more work, time consuming.

## Linux Notes
```
touch [FILE] # Creates an empty file named FILE

```

