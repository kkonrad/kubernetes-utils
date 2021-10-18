# kubernetes-utils
Notes on various utilities for working with K8S.


## Alias

Can be added to your shell rc file
```sh
alias kc=kubectl
```
ex.

```sh
echo -e "\nalias kc=kubectl\n" >> ~/.zshrc
```

## Tools


### Accessing cluster

#### Telepresence

[Telepresence](https://www.telepresence.io/) enables you to quickly connect and access services, pods etc. from your local machine as if you were running in Kubernetes cluster.
It is **AWESOME** tool!
Some time ago I was hitting ocasional crashes (resulting in telepresence pods staying up in a cluster), but with newer version it seems to be fixed.

It is very useful if you:

* don't want to expose your apps to external world, but still would like to access them (do the demo, etc.)
* during development, if you don't know / can't set up locally all dependencies (ex. some data bases, microservices developed by other teams).

Tip: I was using it mostly in a `while` loop in bash so that it quickly recovers in case of any crash / interruption.


### Kubectl plugins

#### TODO: Krew

[Krew](https://krew.sigs.k8s.io/) is a plugin manager for kubectl.

Some plugins to consider:

* ctx
* ns

Now I'm testing:
* access-matrix
* node-shell
* sniff


### Console

#### K9s

[K9s](https://k9scli.io/) works in terminal.
Used it only few times and it looked like early days for this product:

* hit some glitches
* got a little bit lost few times
* couldn't find some relevant info in documentation

In general looks promissing and I plan to get back to it in some time.


### GUI

#### TODO: K8S lens

[Lens](https://k8slens.dev/) claims to be Kubernetes IDE.

Havent used yet - TODO
