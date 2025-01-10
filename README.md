# veld_code__analyse_conllu

This repo contains a code veld that generates a statistical summary on conllu data, to count 
linguistic features of a conllu file:
- count of total tokens 
- count of total lemma
- count of lemma normalized by token (to put the lemma in relation with token)
- count of occurrence of each (Universal Dependencies) part of speech tag

The code veld yaml and more detail within can be found here: [./veld.yaml](./veld.yaml)

Can be adapted to other use cases and made more flexible, but is primarily used in this chain veld: 
https://github.com/veldhub/veld_chain__eltec_udpipe_inference

