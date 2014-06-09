How to Provision a Deis Controller on Digital Ocean
===================================================

Here are the steps to get started on Digital Ocean:

* Get a etcd discovery URL at https://discovery.etcd.io/new and enter it in
  ../coreos/user-data

* Install DO command line client and authorize:

```
gem install tugboat
tugboat authorize
```
You can leave all but the client and API keys as the defaults.

* Find out about the ID of your ssh key (import it into DO if it's not listed):

```
tugboat keys
```

* Create a controller image:

```
./provision-digitalocean-controller-image.sh <YOU SSH KEY ID>
```

* Deploy controllers (odd number) using the newly created image, either via UI
  or tugboat:

```
tugboat create deis1 -r <REGION_ID> -i <IMAGE_ID> -p true -k <SSH_ID> -s 66
```

* Not all regions allow private networks. Better choose one which does.