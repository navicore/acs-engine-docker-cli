# acs-engine-dockerfile
a dockerfile for az, kubectl, and acs-engine

see https://github.com/Azure/acs-engine

useful alias for bash/zsh:

```console
alias acs-engine='docker run -v `pwd`:/files -it navicore/acs-engine'
alias az='docker run --entrypoint /usr/local/bin/az -v `echo $HOME/.azure`:/root/.azure -v `pwd`:/files -it navicore/acs-engine'
#bug! the above 2 commands work but not the kubectl below ?????????? zsh never starts
#alias kubectl='docker run --entrypoint /usr/local/bin/kubectl -v `echo $HOME/.kube`:/root/.kube -v `pwd`:/files -it navicore/acs-engine'
```

