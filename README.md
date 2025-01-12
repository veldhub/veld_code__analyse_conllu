# veld_code__analyse_conllu

**work in progress**

This repo contains [code velds](https://zenodo.org/records/13322913) encapsulating creation of 
statistical summary on conllu data. For now, these are:
- count of total tokens 
- count of total lemma
- count of lemma normalized by token (to put the lemma in relation with token)
- count of occurrence of each (Universal Dependencies) part of speech tag

Can be adapted to other use cases and made more flexible, but is primarily used in this chain veld: 
https://github.com/veldhub/veld_chain__eltec_udpipe_inference

## code velds

- [./veld.yaml](./veld.yaml) : Launches a jupyter notebook providing statistical analysis

## requirements

- git
- docker compose (note: older docker compose versions require running `docker-compose` instead of 
  `docker compose`)

## how to use

A code veld may be integrated into a chain veld, or used directly by adapting the configuration 
within its respective yaml file and using the template folders provided in this repo.

Then, run a veld with:
```
docker compsoe -f <VELD_NAME>.yaml up
```

e.g. 
```
docker compsoe -f veld.yaml up
```


