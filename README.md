This is a bitcoin bech32 vanity address generator written in rust. Bech32 addresses are 'bc1q' started segwit native addresses specified by BIP 0173.   

## Usage

In the following example, we are searching for an address with prefix 'bc1qp2pec', and we finally find that a private key `Kz7QeGuWJMYweKxgUVskDHkw4gU9nbCkd2qnAtEjwVhQHxmub1uL` can producer an address `bc1qp2pecff5tgvzrqkx7ktnv3xazj4l2dcm8e2nae` which satisfies the condition.   

```
# Since all bech32 addresses start with 'bc1q', so here we try to find an address with prefix 'bc1qp2pec'
 $ cargo run --release p2pec  
    Finished release [optimized] target(s) in 0.02s
     Running `target/release/bitcoin-address-prefix-searcher p2pec`
checking prefix bc1qp2pec
count: 550000	elapsed: 0.05min	speed: 171499.84/s	progress(est): 1.64%	left(est): 3.21min
count: 1150000	elapsed: 0.11min	speed: 169816.89/s	progress(est): 3.43%	left(est): 3.18min
count: 1750000	elapsed: 0.17min	speed: 170134.16/s	progress(est): 5.22%	left(est): 3.12min
count: 2350000	elapsed: 0.23min	speed: 170031.11/s	progress(est): 7.00%	left(est): 3.06min
count: 2950000	elapsed: 0.29min	speed: 168967.29/s	progress(est): 8.79%	left(est): 3.02min
count: 3550000	elapsed: 0.35min	speed: 168150.81/s	progress(est): 10.58%	left(est): 2.97min
count: 4150000	elapsed: 0.41min	speed: 167446.74/s	progress(est): 12.37%	left(est): 2.93min
count: 4760000	elapsed: 0.48min	speed: 165634.35/s	progress(est): 14.19%	left(est): 2.90min
count: 5360000	elapsed: 0.55min	speed: 163899.34/s	progress(est): 15.97%	left(est): 2.87min
count: 5960000	elapsed: 0.61min	speed: 162296.11/s	progress(est): 17.76%	left(est): 2.83min
result:
privkey:	Kz7QeGuWJMYweKxgUVskDHkw4gU9nbCkd2qnAtEjwVhQHxmub1uL
address:	bc1qp2pecff5tgvzrqkx7ktnv3xazj4l2dcm8e2nae
```

