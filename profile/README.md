Welcome to rotur!

# What? Who? Why?

## What is rotur?
Rotur is a project started very recently by:<br>

| <img src="https://avatars.githubusercontent.com/u/92952823?v=4" width="140px"> | <img src="https://avatars.githubusercontent.com/u/107750535?v=4" width="140px"> | <img src="https://avatars.githubusercontent.com/u/73702185?v=4" width="140px"> |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| [Mistium](https://github.com/Mistium)                            | [Bob3rRat20](https://github.com/ThatBeaverDev)                      | [ThePandaDev](https://github.com/ThePandaDever)                     |

Rotur is intended to allow any project that uses the cloudlink system to have a standard for communication between projects.

Rotur will allow for much more integration between turbowarp projects that has almost never been seen before.

## Who is Rotur for?

Rotur is intended mostly for Turbowarp operating systems

The standard should allow for things like crossplay of games between operating systems, or collaborative editing on text editors, running on completely different projects!

I think this could be really really cool if its implemented at a wide scale.

## Why use Rotur?

Rotur's packet formatting is simple but powerful, and has a few advantages over using base cl4.

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

You need not worry though! A sample project i have made handles this whole packet thing for you, (linked here:[download](https://github.com/RoturTW/main/raw/main/Example%20Projects/Rotur_Example_Project.sb3)).

Cant wait to answer any questions or just general discussion about this because i think it could go pretty far.

## Learn more here:
https://github.com/RoturTW/main/wiki


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
