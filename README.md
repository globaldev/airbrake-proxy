TCP proxy for buffering connections to Sentry so that they don't add request latency to reporting applications

## Prerequisites

* [Node.js][node] 0.8.8
* [Redis]

## Install & Setup

Get the code from [GitHub][router]:

    cd ~/Projects
    git clone git@github.com:globaldev/error-proxy.git
    cd error-proxy

Install NodeJS 0.8.8

    brew install n
    n 0.8.8

Installing the dependencies:

    npm install

If an `CERT_UNTRUSTED` error is thrown during `npm install` try:

    npm config set strict-ssl false

Create configuration files by copying the example configuration:

    cp config/config.json.example config/config.json

## Running

    cd ~/Projects/error-proxy
    npm start
