## Xmrig AMDGPU cryptonight (default), cryptonight_v7 or cryptonight-lite
-----

### Run

#### Simpleco.in - Default
```
docker run -ti --rm --name Xmrig-amd-doge \
--device /dev/kfd --device /dev/dri \
izone/xmrig-amd
```
```
```
```
docker run -ti --rm --name Xmrig-amd-doge \
--device /dev/kfd --device /dev/dri \
-e DONATE="1" \
-e ALGORITHM="cryptonight" \
-e POOL="simpleco.in" \
-e PORT="8081" \
-e USER="luvres.7873" \
-e USERPASS="x" \
izone/xmrig-amd
```


#### Nicehash (cryptonight)
```
nvidia-docker run -ti --rm --name Xmrig-amd-nicehash \
--device /dev/kfd --device /dev/dri \
-e DONATE="1" \
-e ALGORITHM="cryptonight" \
-e POOL="cryptonight.eu.nicehash.com" \
-e PORT="3355" \
-e USER="3PThBqHfb1UVcZaZXtPAY4SC4fZNBNqCs7.1uvr3z" \
-e USERPASS="x" \
izone/xmrig-amd
```

#### Minergate XMR
```
nvidia-docker run -ti --rm --name Xmrig-amd-Minergate \
--device /dev/kfd --device /dev/dri \
-e DONATE="1" \
-e ALGORITHM="cryptonight" \
-e POOL="xmr.pool.minergate.com" \
-e PORT="45700" \
-e USER="1uvr3z@gmail.com" \
-e USERPASS="x" \
izone/xmrig-amd
```

#### XMR Monero
```
docker run -ti --rm --name Xmrig-amd-XMR \
--device /dev/kfd --device /dev/dri \
-e DONATE="1" \
-e ALGORITHM="cryptonight" \
-e POOL="pool.supportxmr.com" \
-e PORT="5555" \
-e USER="43oMPyqNyYmP5S4gatvSPKPLD2ysjpdyq63BJx2JWUjHVVCTFTn4ccy9LC1cGGUvApCdCGrECuSf9eo2WHBckfBxNx9Dqkf" \
-e USERPASS="fx8350" \
izone/xmrig-amd
```

#### BBS Coin (cryptonight_v7)
##### Web Wallet
```
docker run -ti --rm --name Xmrig-amd-BBS \
--device /dev/kfd --device /dev/dri \
-e DONATE="1" \
-e ALGORITHM="cryptonight_v7" \
-e POOL="pool.bbscoin.xyz" \
-e PORT="5555" \
-e USER="fyTo1z3Cw961pVVyxjmYGjW3hXipzT6q3gzYCnWpBGAv7tYYgTdt4WfKEBpzjVZ8UgjFAn3iLBnoCB8VzNjpPVjL25J8AyW3E" \
-e USERPASS="x" \
izone/xmrig-amd
```
##### Local Wallet
```
docker run -ti --rm --name Xmrig-amd-BBS \
--device /dev/kfd --device /dev/dri \
-e DONATE="1" \
-e ALGORITHM="cryptonight_v7" \
-e POOL="pool.bbscoin.xyz" \
-e PORT="5555" \
-e USER="fyTZ7jLeycCEYMpexDcUMCaxiErw7mFJDNMAJNShyWRA1dnf7ZmHgj8Zwd61VKiEjHDd8TsgZJL9h4ZdbYBdfCHv32d62EsgX" \
-e USERPASS="x" \
izone/xmrig-amd
```

-----
#### Build
```
docker build -t izone/xmrig-amd .
```
```
docker build -t izone/xmrig-amd:build -f Dockerfile_build .
```

