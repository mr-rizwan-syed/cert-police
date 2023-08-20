# cert-police

# CertPolice

CertPolice is a Bash script for monitoring real-time Certificate Transparency (CT) logs, extracting domain names from these logs, matching them against specified domains/keywords, and sending notifications if matches are found.

## Features

- **Real-time Monitoring:** CertPolice continuously monitors CT logs in real time, ensuring timely detection of new certificates.
- **Domain Extraction:** It extracts domain names from CT logs and identifies subdomains associated with these certificates.
- **Customizable Matching:** Match extracted subdomains/domains against a list of target domains or keywords.
- **Silent Mode:** Run in silent mode to suppress unnecessary output.
- **Notification Support:** Optionally enable notifications using the `notify` tool to receive alerts for matching domains.
- **Dependency Management:** Automatically checks and installs necessary dependencies if missing.
- **Informative Output:** Provides clear output indicating found subdomains and matches.


## Installation

   ```bash
   git clone https://github.com/mr-rizwan-syed/CertPolice.git
   cd CertPolice
   chmod +x certpolice.sh
   ./certpolice.sh -t targets.txt
   ```

## Usage

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


Cert-Police is a rewritten in Bash script from the Python codebase of [CertEagle](https://github.com/devanshbatham/CertEagle), addressing the original project's Slack-only limitation.<br>
A special thanks to [Devansh Batham](https://github.com/devanshbatham) for the inspiration from their original project idea in [CertEagle](https://github.com/devanshbatham/CertEagle).
