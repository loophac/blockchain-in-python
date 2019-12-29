# Blockchain in Python

This work is based on [adilmoujahid/blockchain-python-tutorial](https://github.com/adilmoujahid/blockchain-python-tutorial).


## Novel Features

Compared with the original one, we now introduce:

- Constant wealth (`1e8` coin in total).
- Setting miner's information.
- Balance check before every transaction.
- Transaction failure alert.
- Dynamic `difficulty` update every 2 weeks.
- SSL support.
- Save running sates.



(Risky, not recommended) If you need SSL support, add certificate(inside `certificates` folder) to your system(`cert.pem`) or your browser(`cert.p12`). 


## Requirements

In order to run this code, you'll need:

- python 3
- pycrypto

To install the pycrypto:

```
pip instal pycrypto
```


## Usage



To run blockchain node:

```bash
python blockchain/blockchain.py -p 5000
```

which we also support restoring to previous state with `-r path\to\file.pkl`.
The default file of state is stored in `states\blockchain.pkl`.

To run blockchain client:

```bash
python blockchain_client/blockchain_client.py -p 8080
```
