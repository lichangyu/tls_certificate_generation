# Renew or create let's encrypt certificates using temporary AWS / DO machines  #

### Steps ###

* Make sure you have docker installed
* Configure your domains at `nginx/sites-enabled/site.conf`
* For AWS usage
  * Run `EC2_AKEY=xxx EC2_SKEY=yyy EC2_VPCID=kkk ./renew.sh` and follow the steps (like configuring DNS and etc)
* For DO usage
  * Run `DO_ATOKEN=xxx ./renew.sh digitalocean` and follow the steps (like configuring DNS and etc)
* Get the certificates `privkey1.pem` and `fullchain1.pem`.
