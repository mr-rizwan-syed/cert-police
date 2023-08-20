# cert-police

```
└─# ./cert-police.sh

Certificate Transparency Monitoring @_r12w4n

./cert-police.sh --silent --notify --target targets.txt
./cert-police.sh -s -n -t target.txt
./cert-police.sh --add STRING --target targets.txt
./cert-police.sh -a STRING -t targets.txt
```
## Configure notify 
In order to get alerts, you need to configure notify
The default provider config file of notify created at $HOME/.config/notify/provider-config.yaml

![cert-police_usage](https://i.imgur.com/mgbPgm0.png)
