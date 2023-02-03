# my_coin

## aptos init

- mod와 private key 설정

```
aptos move init
```

## test

```
aptos move test
```

## setting

```
[package]
name = 'my_coin'
version = '1.0.0'
[dependencies.AptosFramework]
git = 'https://github.com/aptos-labs/aptos-core.git'
rev = 'main'
subdir = 'aptos-move/framework/aptos-framework'
[addresses]
BlockSec = "0xaddress"
```

- 1APT add

```
aptos account fund-with-faucet --account *address*
```

## deploy

```
aptos publish

```

## testnet

```
 aptos node run-local-testnet --with-faucet --force-restart
```

## aptor copile

```
aptos move compile
```
