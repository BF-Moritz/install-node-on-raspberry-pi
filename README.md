# install-node-on-raspberry-pi
A guide to install NodeJS on a raspberry pi

# update your pi

Before we install anything on your pi, it is recommendet to update all existing software on it.
For this just run:

```bash
sudo apt-get update
```

To upgrade all software to the latest version, run

```bash
sudo apt-get upgrade 
```

Now we are ready to install new packages.

# install node

First we have to add the NodeSource repository to our package manager. 
We do this with this command:

```bash
curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
```

Then we can install node with our package manager.

```bash
sudo apt-get install -y nodejs
```

To confirm, that NodeJS was successfully installed, we can run the following command:

```bash
node -v
```

The answer should be the version of node installed (example:`v16.11.1`)
