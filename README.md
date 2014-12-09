ocs-scripts
===========

This repository contains the scripts used to boot an image on [Online.net's cloud services](http://labs.online.net/).
Scripts are built-in official images and some of them are also used in the official Initrd image.

It is planned to to create packages (.deb) for distributions.

---

The official images built with [image-tools](https://github.com/online-labs/image-tools) are using this repositoty.
(i.e. [Ubuntu](https://github.com/online-labs/image-ubuntu), [Debian](https://github.com/online-labs/image-debian), [Docker app](https://github.com/online-labs/image-app-docker), [Wordpress app](https://github.com/online-labs/image-app-wordpress), ...

Upgrade a running image
-----------------------

```bash
wget -qO - http://j.mp/ocs-scripts | bash
```

Using flavors
-------------

```bash
# upstart
wget -qO - http://j.mp/ocs-scripts | FLAVORS=upstart bash
```

```bash
# sysvinit
wget -qO - http://j.mp/ocs-scripts | FLAVORS=sysvinit bash
```

Using branches
--------------

```bash
# flavor=upstart on branch=feature-xxx
wget -qO - http://j.mp/ocs-scripts | FLAVORS=upstart BRANCH=feature-xxx bash
```

You can also use this url https://raw.githubusercontent.com/online-labs/ocs-scripts/master/upgrade_root.bash instead of http://j.mp/ocs-scripts
