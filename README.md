# MySQL 5.7 ARM Docker

**This is not a multiarch docker!**

Sadly the MySQL 5.7 arm64 packages were built but not pushed to the official repositories nor the security team's PPA so I need to download the `deb` files manually from Launchpad with wget and install with dpkg (apt doesn't work due to some `deb` headers misconfigured).


## Building this project

First git clone it to your machine.

Afterwards run the following command:

```bash
docker buildx build --platform=linux/arm64 .
```

Good luck!
