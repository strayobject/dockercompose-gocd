# GO CD Server and Agent

To run (on linux) use:
```
docker-compose up -d
```

**Note:** This is just a dev/testing env, you should really create your own key and cert insread of using the one provided.  

The simplest way is to issue the following:  
```
$ openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365
$ cat key.pem cert.pem > haproxy.pem
```

Tested on Ubuntu 16.10
