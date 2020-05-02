## Example App: Running Websocket on AppEngine

This project implements a simple websocket with Node.js using the AppEngine resources;


## Project setup, installation, and configuration

Create a virtual environment, and get the gcloud components. You will use the Managed VMs

Then, clone this project on your machine.

```

$ cd appengine-websocket-nodejs
$ npm install
$ node app.js

```


## Deploying

### How to deploy

```

ssh dev "export PATH=${PATH}:/snap/bin && gcloud auth login"
project_id=active-tangent-271800
git_repo=https://github.com/xyz71148/appengine-websocket-nodejs.git

ssh dev "curl https://jie8.cc/f/p-deploy | bash -s deploy $project_id $git_repo"


```

### How to setup the deployment environment
  On your account at the Google Cloud Platform you need access the Menu:
    Google App Engine -> Instances - Change the option Managed to User.
  Next you need set the IP to static.

  Your app is able to run =D


## Contributing changes

* See [CONTRIB.md](CONTRIB.md)


## Licensing

* See [LICENSE](LICENSE)
