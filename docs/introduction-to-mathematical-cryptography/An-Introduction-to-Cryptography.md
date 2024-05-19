# An Introduction to Cryptography

## 1.1 Simple Substitution Ciphers

Caesar is a simple substitution cipher which shifts every letter by a specific number (for example 5)

jsjrdkfqqnslgfhpgwjfpymwtzlmnrrnsjsyqzhnzx
enemyfallingbackbreakthroughimminentlucius

![Figure 1.1](./imgs/Screenshot 2024-05-17 at 2.19.39 AM.png)

simple substitution may differ from caesar (shift cipher) to random mapping

#math
```
{a,b,c,d,e,...,x,y,z} −→ {A,B,C,D,E,...,X,Y,Z}
```

we can create encryption and decryption table to make encryption and decryption processes more convinient

![Table 1.1 ,1.2](./imgs/Screenshot 2024-05-17 at 2.27.31 AM.png)


### 1.1.1 Cryptanalysis of Simple Substitution Ciphers

how many simple substitution ciphers?

#math
```
26*25*24*...*3*2*1 = 26! = 403291461126605635584000000
```

sthere are a lot of possible keys for Eve to break Alice and Bob encrypted message. it takes `10^10` years if she can try 1 million keys per second. so this looks impossible. right?

#quote
```
Your opponent always uses her best strategy to defeat you, not the strategy that you want her to use. Thus the security of an encryption system depends on the best known method to break it. As new and improved methods are developed, the level of security can only get worse, never better.
```


letters in english are not random. for example letter `e` is much more frequent and e is mostly followed by `t,a,o,n` and `q` is usually followed by `u` and it is unlinkely to see letters `fc` beside eachother.

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.18.04 AM.png)


the goal of decryption a simple substitution cipher is not decrypting the cipher text but it is introducing a new idea named statistical analysis in terms of cryptanalysis.

an example

```
LOJUM YLJME PDYVJ QXTDV SVJNL DMTJZ WMJGG YSNDL UYLEO SKDVC
GEPJS MDIPD NEJSK DNJTJ LSKDL OSVDV DNGYN VSGLL OSCIO LGOYG
ESNEP CGYSN GUJMJ DGYNK DPPYX PJDGG SVDNT WMSWS GYLYS NGSKJ
CEPYQ GSGLD MLPYN IUSCP QOYGM JGCPL GDWWJ DMLSL OJCNY NYLYD
LJQLO DLCNL YPLOJ TPJDM NJQLO JWMSE JGGJG XTUOY EOOJO DQDMM
YBJQD LLOJV LOJTV YIOLU JPPES NGYQJ MOYVD GDNJE MSVDN EJM
```

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.48.36 AM.png)

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.48.49 AM.png)

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.49.10 AM.png)

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.49.20 AM.png)

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.49.28 AM.png)

![Table 1.1](./imgs/Screenshot 2024-05-17 at 2.49.32 AM.png)


```
The writer claimed by a momentary expression, a twitch of a mus- cle or a glance of an eye, to fathom a man’s inmost thoughts. His conclusions were as infallible as so many propositions of Euclid. So startling would his results appear to the uninitiated that until they learned the processes by which he had arrived at them they might well consider him as a necromancer.
```