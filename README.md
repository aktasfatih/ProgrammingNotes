## Github
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - It is the best fource for learning Markdown syntax that Github uses.
- [Github Formatting](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#quoting-code) - Official Docs for Github's formatting.
- [Continous Deployment](https://hackernoon.com/continuous-deployment-with-aws-codedeploy-github-d1eb97550b82)
- [More CI/CD](https://medium.com/@mosheezderman/how-to-set-up-ci-cd-pipeline-for-a-node-js-app-with-jenkins-c51581cc783c)
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
- [Main login workflow Express and RN](https://appdividend.com/2018/02/07/node-js-jwt-authentication-tutorial-scratch/)

## ReactNative
- [Redux, Tutorials point](https://www.tutorialspoint.com/redux/redux_installation.htm)
- [Immutable](https://immutable-js.github.io/immutable-js/) - Helps with immutable objects in RN
- [Best Redux Example](https://redux.js.org/basics/reducers) - Use the **reducer composition** format
- [Auth with Mongoose and Facebook](https://alexanderpaterson.com/posts/add-social-authentication-to-a-react-native-application)

**Reducer Composition**: Each reducer is responsible of its own part in the state. For example, local state equals the state of the App.js.

## Linux Notes
```
touch [FILE] # Creates an empty file named FILE

```

## Computer Science AWS
- [Data Structures](https://medium.com/swlh/introduction-to-data-structures-9134b7d064a6) - A summary of data structures
- [Setting up VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)

