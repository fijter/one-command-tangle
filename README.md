One command private test Tangle
================================

This repository provides you with a way to set up a development/testing IOTA network using a single command.
It installs a IRI docker container and a Compass docker container. It also includes a pre-built merkle tree with a depth of 20,
Enough to let a network run for over a year.

## Warning

The sole purpose of this is to set up a quick testnet; It uses a pre-shared merkle tree and Coordinator seed. Do not use this for
anything else besides local testing since it would be insecure to use this otherwise.

## Getting started

1. Make sure you have `docker` and `docker-compose` installed on your local machine
2. Within this folder execute `docker-compose up`
3. Enjoy your private tangle!

## Notes

- With the default settings all 2.7Pi on this testnet will be available on the seed `SEED99999999999999999999999999999999999999999999999999999999999999999999999999999`
- If you want to start Compass again after stopping it make sure to remove the `-bootstrap` line from `docker-compose.yml` before starting again.
