# chef-server-box
chef-server-box is utility tools for serving Chef Server.

## What is included?
This docker image include
- Ruby 2.0.0
- Chef Server (use [base/chef-server](https://github.com/tmc/dockerfiles/tree/master/chef-server))
- Chef Client
- Berkshelf API Server
- SSH Server

Running processes on a container by Supervisor
- sshd
- chef-server
- berkshelf-api

## Usage
```
> docker run -d -p 443:443 -p 10022:22 -p 26200:26200 foostan/chef-server-box
```

## Contributing
1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
