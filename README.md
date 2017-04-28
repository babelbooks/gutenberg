# gutenberg
Meta Repository for Babel books. Please do not work in this repository, instead use the individual git

## How to install
1. Clone this repository: `git clone https://github.com/babelbooks/gutenberg.git`
2. Init submodules: `git submodule update --init --recursive`
3. Deploy it with the master docker-compose file.

    Please note that `printer` is a bit tricky to build.
    So an extra step is needed to compose:
    
    ```
    cd printer
    npm run deploy
    cd ..
    docker-compose up
    ```
    
    NOTE: If you want to **re**build it, don't forget to add `--build` to the docker-compose command.

## Update the git submodules
This command will update all the submodules in this repository:
```
git submodule update --recursive --remote
```

Please note that this will only work if you have initialized submodules.

