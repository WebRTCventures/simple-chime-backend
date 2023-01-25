# Simple Amazon Chime SDK Application
## Backend

> Very simple video conference app using AWS Chime.

For setting up, make sure you have **Node 16** and a **AWS profile with Chime access configured** using your AWS CLI. Then download the dependencies and run the development server with this command:

```sh
npm install
```

Generate an env file, a copy from `sample.env` but called `.env`, like this:

```sh
cp sample.env .env
```

Generate an ARN for your application, here's an example using your configured AWS CLI:

```sh
aws chime-sdk-identity create-app-instance --name simple-chime-app
```

Take note of the outputted ARN and use it to fill that `.env` file you just created, along with
your AWS credentials.

And then run the development server:

```sh
npm start
```

Now go make [the frontend](https://github.com/WebRTCventures/simple-chime-frontend) work too after this.
