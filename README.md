# 🦅 De Minimis HawkScan

This repo contains the simplest possible HawkScan configuration. All you need to provide is a StackHawk Application ID and API key.

## What's In the Box

This repo contains the following active ingredients:
- `stackhawk.yml`: A minimal StackHawk HawkScan configuration, including application ID, target host, and environment name.
- `docker-compose.yml`: A Docker Compose file to codify a HawkScan run. It pulls the HawkScan container and runs it with environment variables you supply to pass along your application ID and API key.

## Running

1. Sign up for a free trial of [StackHawk](https://auth.stackhawk.com/signup). In the initial setup, record your initial API Key and Application ID.
1. Install [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/)
1. Clone this repository to your machine
    ```
    git clone https://github.com/kaakaww/simple-scan.git
    cd simple-scan
    ```
1. Export your API Key and Application as environment variables.
    ```
    export API_KEY=<your API key here>
    export APP_ID=<your App ID here>
    ```
1. Run HawkScan!
    ```
    docker-compose up
    ```
