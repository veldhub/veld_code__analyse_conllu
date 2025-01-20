# ![veld chain](https://raw.githubusercontent.com/veldhub/.github/refs/heads/main/images/symbol_V_letter.png) veld_code__analyse_conllu

**\*work in progress\***

This repo contains [code velds](https://zenodo.org/records/13322913) encapsulating creation of 
statistical summary on conllu data. For now, the observed features are:
- count of total tokens 
- count of total lemma
- count of lemma normalized by token (to put the lemma in relation with token)
- count of occurrence of each (Universal Dependencies) part of speech tag

The code can be adapted to other use cases but is primarily used in this chain veld: 
https://github.com/veldhub/veld_chain__eltec_udpipe_inference

## requirements

- git
- docker compose (note: older docker compose versions require running `docker-compose` instead of 
  `docker compose`)

## how to use

A code veld may be integrated into a chain veld, or used directly by adapting the configuration 
within its yaml file and using the template folders provided in this repo. Open the respective veld 
yaml file for more information.

**[./veld.yaml](./veld.yaml)** : Launches a jupyter notebook providing statistical analysis
```
docker compose -f veld.yaml up
```

