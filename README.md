# gutenberg
Meta Repository for Babel books. Please do not work in this repository, instead use the individual git

## How to install
1. Clone this repository: `git clone https://github.com/babelbooks/gutenberg.git`
2. Init submodules: `git submodule update --init --recursive`
3. Deploy it with the master docker-compose file.

    To ensure that everything is ok, it's better to use our packaged command:
    
    ```
    npm start
    ```
    
    NOTE: By default, the command above doesn't rebuild images if not needed and doesn't run as a deamon.
    If you want to **re**build it and/or run it as deamon, use one of these commands instead:
    
    ```
    npm run rebuild
    npm run daemon
    npm run daemon-rebuild
    ```

## Update the git submodules
This command will update all the submodules in this repository:
```
git submodule update --recursive --remote
```

Please note that this will only work if you have initialized submodules.

