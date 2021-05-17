# SushiOrPizza
which one is my favorite food?

## Quick demo thing to learn signing / verifying messages
How to determine which one of the messages is the real one:

```
    git clone https://github.com/melvyniandrag/SushiOrPizza.git
    cd SushiOrPizza/
    gpg2 --import melvyn.pubkey.gpg
    gpg2 --verify favfood.1.txt.sig 
    gpg2 --verify favfood.2.txt.sig 
```

one of the --verify commands will say "Good signature", the other one will say "BAD signature". If favfood.1.txt.sig is the good one, then have a look in favfood.1.txt.
If favfood.2.txt.sig is the good one, then you can trust favfood.2.txts
