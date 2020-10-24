# ink-vscode-remote

### Creating a new contract

```
cargo contract new flipper
```


### Testing contract

```
cargo +nightly test
```

### Compiling and Building Contract

```
cargo +nightly contract build
```

### Generate ABI and metadata

```
cargo contract generate-metadata
```

### Starting node for deploy and test
```
canvas --dev --tmp --ws-port=9944
```

Go to remote explorer in vs code and forward the port 9944.