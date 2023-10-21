# Remotion videos

My personal repo of Remotion videos I make.

Started from [this repo](https://github.com/JonnyBurger/contribution-graph).

## Setup

Using [Bun](https://bun.sh/).

```
bun i
```

## Run

```
bun dev
```

Open http://localhost:3000

### Opens Remotion Studio

```
bun run remotion
```

### Deploy to AWS

```
node deploy.mjs
```

You should run this script after:

- changing the video template
- changing `config.mjs`
- upgrading Remotion to a newer version

### Set up rendering on AWS Lambda

Can also render videos via [Remotion Lambda](https://remotion.dev/lambda).

1. Copy `.env.example` file to `.env` and fill in the values.
   Complete the [Lambda setup guide](https://www.remotion.dev/docs/lambda/setup) to get your AWS credentials.

1. Edit `config.mjs` file to your desired Lambda settings.

1. Run `node deploy.mjs` to deploy your Lambda function and Remotion Bundle.
