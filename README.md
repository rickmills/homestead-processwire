# Homestead Processwire Support
This package provides a boot script for Laravel Homestead, adding support for Processwire CMS.

## What it does
The included shell script provides homestead with a set of server configuration commands to support things like URL Rewriting and SSL. By extension, this also makes Processwire compatible with Nginx, which is the default web-server in a Homestead vagrant box.

## How to use it
1. Download (or checkout) the included `serve-processwire.sh` file into your `Homestead/scripts/` directory - you'll see many other platform shell scripts here.

2. Open your `Homestead.yaml` file and modify the host for your processwire installation to include a type of `processwire`.

Example:

```
- map: processwire.site
- to: /home/vagrant/code/processwire
- type: processwire
```

That's it!
