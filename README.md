# Ethereum Toolbox

## Run Embark demonstration

```shell
$embark demo
$cd /embark_demo
$embark blockchain
```

```shell
$docker run --name dapp -d -v /dapp jlrigau/embark demo
$docker run --name blockchain -d --volumes-from dapp -p XXXX:XXXX jlrigau/embark blockchain
```
