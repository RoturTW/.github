Welcome to Rotur!

# What? Who? Why?

## What is rotur?
Rotur is a project started on the 29th of June, 2024 by these people:<br>

| <img src="https://avatars.githubusercontent.com/u/92952823?v=4" width="140px"> | <img src="https://avatars.githubusercontent.com/u/178028063?s=200&v=4" width="140px"> | <img src="https://avatars.githubusercontent.com/u/73702185?v=4" width="140px"> |
| :----------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------: | :----------------------------------------------------------------------------: |
|                     [Mistium](https://github.com/Mistium)                      |              [The Constellinux Project](https://github.com/Constellinux)              |                [Flufi](https://github.com/ThePandaDever)                 |

Rotur is intended to allow any project that uses the cloudlink system to have a standard for communication between projects.

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
        "payload": "", // the data that you are sending to the port
        "timestamp": "" // the unicode timestamp of when the packet was sent
    },
    "id": "" // username to send the packet to
}
```

You need not worry though! A sample project we have made handles this whole packet thing for you, (linked here:[download](https://raw.githubusercontent.com/RoturTW/main/main/Implementations/SCRATCH/Rotur_Example_Project.sb3)).

Cant wait to answer any questions or just general discussion about this because i think it could go pretty far.

## Links:
https://rotur.dev
https://github.com/RoturTW/main
