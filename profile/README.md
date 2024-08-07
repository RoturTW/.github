Welcome to rotur!

# What? Who? Why?

## What is rotur?
Rotur is a project started on the 29th of June, 2024 by these people:<br>

| <img src="https://avatars.githubusercontent.com/u/92952823?v=4" width="140px"> | <img src="https://avatars.githubusercontent.com/u/107750535?v=4" width="140px"> | <img src="https://avatars.githubusercontent.com/u/73702185?v=4" width="140px"> |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| [Mistium](https://github.com/Mistium)                            | [ThatBeaverDev](https://github.com/ThatBeaverDev)                      | [ThePandaDev](https://github.com/ThePandaDever)                     |

Rotur is intended to allow any project that uses the cloudlink system to have a standard for communication between projects.

Rotur allows for much more integration between turbowarp projects that has almost never been seen before.

## Who is Rotur for?

Rotur is intended mostly for Turbowarp operating systems

The standard should allow for things like crossplay of games between operating systems, or collaborative editing on text editors, running on completely different projects!

We think this could be really really cool if its implemented at a wide scale, and it is currently Present in 5 Systems (2 Released)

## Why use Rotur?

Rotur's packet formatting is simple but powerful, and has a few advantages over using base [Cloudlink 4](https://github.com/MikeDev101/cloudlink), which is for Scratch-Based Mods.

This is a raw packet sent from 
```js
{
    "cmd": "pmsg", // yes this is based on cl4
    "val": {
        "client": { // some metadata info (kinda like the user agent)
            "system": "", // name of the system you are using
            "version": "" // version of the system you are using
        },
        "source": "", // this is the port you are sending the data from (to allow for replies)
        "target": "", // this is the 'port' that you want to send to
        "payload": "" // the data that you are sending to the port
    },
    "id": "" // username to send the packet to
}
```

You need not worry though! A sample project we have made handles this whole packet thing for you, (linked here:[download](https://raw.githubusercontent.com/RoturTW/main/main/Implementations/SCRATCH/Rotur_Example_Project.sb3)).

Cant wait to answer any questions or just general discussion about this because i think it could go pretty far.

## Learn more here:
https://github.com/RoturTW/main

# What can I use to make clients?

Rotur is able to be used on any one of the clients below, click the link to be taken to a page with code you can easily copy and paste to get your own client setup quickly!

| <img src="https://avatars.githubusercontent.com/u/67349469?s=200&v=4" width="140px"> | <img src="https://raw.githubusercontent.com/Mistium/Origin-OS/main/Resources/origin-logo-new.png" width="140px"> | <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/600px-JavaScript-logo.png" width="140px"> | <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1869px-Python-logo-notext.png" width="140px"> |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:-------------------------------------------------------------------:|:----------------------------------------------------------:|
|[Turbowarp](https://github.com/RoturTW/main/tree/main/Implementations/SCRATCH)|       [OSL](https://github.com/RoturTW/main/tree/main/Implementations/OSL)      |   [Javascript](https://github.com/RoturTW/main/tree/main/Implementations/JS)    | [Python](https://github.com/RoturTW/main/tree/main/Implementations/PY) |

# Documentation:

## Information:

### Setup
This is for the initial setup of Rotur

[How to Get Connected](https://github.com/RoturTW/main/wiki/Connecting-to-Rotur)

---

### Packets
The way that packets are structured on Rotur uses cloudlink as a base and passes more information between clients about the connection and about the user thats connected as well as allowing more specific targeting of packets within the project using a "port" targeting system.

[Packet Structure](https://github.com/RoturTW/main/wiki/Packet-Structure)

---
### The Client
Handling incoming packets and sending packets can be kinda tricky so we set out a guide for the formatting and the blocks you need to put together for the best and most reliable client

Its best to use the client from the example project at the top of this page
---
### Usernames
A rotur designation is the way that a username is formatted to tell other clients, what system is being used by that user

[Rotur Designations](https://github.com/RoturTW/main/wiki/Rotur-Designations)
