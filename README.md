WalletConnect v2.x.x

Open protocol for connecting Wallets to Dapps - https://pbnc.me
Setup development

The following dependencies are required for relay server:

    git
    npm
    make
    nodejs
    docker version 20.10

To setup the local redis and relay server you can run:

make dev

Test Client

Client unit tests can be run against: local (make dev), staging, and production server

# local (dev)
make test-client

# staging server
make test-staging

# production server
make test-production

Additional help

bootstrap-lerna      setups lerna for the monorepo management
build-react-app    builds the example react-app
build-react-wallet builds the example react-wallet
build-container      builds relay docker image
build-lerna          builds the npm packages in "./packages"
build-nginx          builds nginx docker image
build                builds docker images
clean-all            cleans lerna bootstrap
clean                removes all build outputs
cloudflare           setups cloudflare API token secret
config               configures domain and certbot email
deploy-monitoring    same as deploy but also has monitoring stack
deploy               deploys production stack with './config' file contents
dev                  runs relay on watch mode and shows logs
help                 Show this help
pull                 downloads docker images
redeploy             redeploys the prodution containers and rebuilds them
relay-logs           follows the relay container logs. Doesn't work with 'make dev'
reset                removes config and lerna bootstrap
rm-redis             stops the redis container
start-redis          starts redis docker container for local development
stop                 stops the whole docker stack
test-relay           runs "./servers/relay" tests against the locally running relay. Make sure you run 'make dev' before.
test-client          runs "./packages/client" tests against the locally running relay. Make sure you run 'make dev' before.
test-production      tests client against pbnc.me
test-staging         tests client against pbnc.me

License

Apache 2.0
