# connectionless-mq
Imagen a connectionless message queue... yeah keep imagening.

im still working on this its just that im doing other stuff and work is eating alot of time.

So i have been a bit sidetracked, i have been investigating message queues and streaming systems i like.
Currently i like NATS-jetstream a lot and how that feels to work with.
* [NATS-server](https://github.com/nats-io/nats-server)

I also found BlazingMQ earlier this week, so im looking at that too see the nice features there.
* [BlazingMQ](https://github.com/bloomberg/blazingmq)


Current thought is to make this in _rust_ i think, becuse i feel like its has more of a future here. 🤔
... shame that i dont know too much of it yet.(something something sidetrack)

## Primary idea.

Create a message queue system or streaming system that is connectionless, like WireGuard,
Initially I had some packets structures I stole from WireGuard and used that to generate payloads to see how it felt.

With the connectionless aspects, I was going to use the `Noise Protocol` like WireGuard, with a similar setup process. 
That way all nodes in a cluster would trust each other and i could skip some access control stuff.

The idea is that you have several clients each with a different key around the place, and they can send messages back and forth,
originally it was part email, part chat and 100% undefined.

But the more I worked on my crude ideas, I realize a message queue or streaming system works best, that way people can send whatever through it.


I have a bunch of smaller junk apps in different languages that implement small parts of this idea, but I won't commit them, I want to keep it clean while I figure out the shape of the thing.
