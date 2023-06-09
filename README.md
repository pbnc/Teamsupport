WalletConnect v2.x.x

Open protocol for connecting Wallets to Dapps - https://walletconnect.com
Setup

    Ensure nodejs and npm
    Clone the repository
    Install all package dependencies, by running npm install from the root folder

Running checks for all packages

To ensure all packages lint, build and test correctly, we can run the following command from the root folder:

    For tests to pass in the following command, you will need your own TEST_PROJECT_ID value, which will be generated for you when you set up a new project on WalletConnect Cloud.

TEST_PROJECT_ID=3c202020928b93669dc500bfd15cadc3 npm run check

Command Overview

    clean - Removes build folders from all packages
    lint - Runs eslint checks
    prettier - Runs prettier checks
    build - Builds all packages
    test - Tests all packages
    check - Shorthand to run lint, build and test commands
    reset - Shorthand to run clean and check commands

Troubleshooting

    If you are experiencing issues with installation ensure you install npm i -g node-gyp
    You will need to have xcode command line tools installed
    If there are issues with xcode command line tools try running

sudo xcode-select --switch /Library/Developer/CommandLineTools
sudo xcode-select --reset

License

Apache 2.0
