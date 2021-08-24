# ethereum-smart-contract-examples

This repo uses [docker-compose](docker-compose.yaml) to start a single node
Ethereum test network using
[Geth's dev mode](https://geth.ethereum.org/docs/getting-started/dev-mode)

## Creating an account

We can connect to the development console using

```bash
docker-compose exec geth geth attach /root/.ethereum/geth.ipc
```

Create a new account (the password can be empty) which will then print out the
address of your new account.

```
> personal.newAccount()
Passphrase:
Repeat passphrase:
"0x380a14ca0a27f6d46b242fe5de29bd158af48d70"
```
