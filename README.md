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

## testnet

```
 aptos node run-local-testnet --with-faucet --force-restart
```

## 계약컴파일

```
aptos move compile
```

## deploy

```
aptos publish

```

## 기본계정 등록

```
aptos move run --function-id 'default::bsc::register'
```

## mint

```
aptos move run  --function-id default::bsc::mint_coin --args address:"발매자" u64:10000000
```

## Transfer

```
aptos move run --function-id 0x1::coin::transfer --type-args *address1*::bsc::BSC --args address:*address2* u64:111
```

## 새로운 계정생성

```
aptos init --profile a2
```

## 새로운 계정 등록

```
aptos move run --profile 0xb76f4caa1c9d95ac20795c19f854ea45f38a8e0a9147300fd0329436543109ec --function-id default::bsc::register
```

## Transfer

```
aptos move run --function-id 0x1::coin::transfer --type-args *address1*::bsc::BSC --args address:*address2* u64:111
```
