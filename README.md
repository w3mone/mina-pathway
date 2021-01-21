# mina-pathway
A place to understand ...how to connect, transact, and build with this language | framework | protocol.

## welcome
If you've just discovered `MINA` or have heard of it before, but didn't know how to get started, this is a good starting point.

There are multiple ways to get started and contribute to the network. Assuming you're a bit technical (or keen) and want to help strengthen the network, you may consider running a `block-producer` node &/or `snark-worker` node.

Check out the MINA protocol main webpage for a quick tour and you'll find a wealth of information here.

[mina-protocol-webpage](https://minaprotocol.com/)

## mina-block-producer node
In the event you want to run a `block-producer` node for the `MINA` network, you'll find the following resource useful.

We will cover 3 topics, how to  **setup**, **run**, and **monitor** your node.

### setup
In terms of setup for running the above node, again, there is no one method. Here are few options you can look into, and based on your preference, you may choose that option.

#### options
1. bare-metal: here you're either renting or purchasing a physical server
2. cloud: here you're renting a virtual computer from any of the providers (e.g. AWS, GCP, Azure, ...)

For the purposes of this tutorial, we are going with option **bare-metal** and a ubuntu linux operating system.

We are also going to assume you know how to install the operating system.

First thing first, log into the machine as `root` super user and 

Create a new user coda

```
adduser coda
```

Grant sudo privileges to this newly created user
```
usermod -aG sudo coda
```

You can logout from `root` user and login as `coda` user

Once logged into the machine as `coda` go ahead and install the latest or appropriate binaries as directed by core team. Join the Discord group and keep an eye on the #announcements | #news-and-updates channels.

Double check to make sure you have the coda binaries available in your machine.

One way to do this is to run the following commands:

C:
```
whereis coda
```
O;
```
coda: /etc/coda /user/local/bin/coda
```

C:
```
coda version
```
O:
```
Commit [DIRTY]5c08d6d51111d31269e77f3c62a544b3262ee4c8 on branch HEAD
```

Note: the ^ release is the latest when this resource was written.


### run

It is a common best practice to automate running your node, such that is functional 24x7 and restarts just in case the machine reboots.

In this example we are going to use **systemd** to automate.

Create a `services` directory in your $HOME and change directory into the newly created directory.
```
cd $HOME
mkdir services
cd services
```

Use your favorite editor (e.g. nano) to create a new services files called `coda.service`. You'll find a working example of coda.service in this repository. Do feel free to use it as-is and/or modify it to suit your needs.

### monitor

[become-a-block-producer](https://minaprotocol.com/docs/node-operator)

## mina-snark-worker-node

## randomising your snark-worker fees

## systemd services

## journalctl services

## monitoring services