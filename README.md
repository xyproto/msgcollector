# Message Collector

A server for collecting messages to the system administrator.
Notes from when installing packages is a good example.

A web, CLI or GUI client provides a good overview of the messages, and the ability to mark messages as read, or clear the message queue.

A notification client can pop up the latest messages, one by one.

The pacman log can be parsed to provide one of many possible streams of notifications, for a transition period.

Hopefully, packages will start communicating directly with the message collector instead of just outputting messages to the terminal.

The messages could also be formatted in a way that:
 * Makes it easy to find relevant information online
 * Makes it easy to know what is "a friendly tip", "nice to know" or "critical information".

Plan:
1. Create an ascii output format that can be interpreted by the message collector.
2. Parse the existing pacman.log files successfully.
3. Make it easy to submit a message from a PKGBUILD or .install file to the message collector.
4. Create several beautiful clients that makes reading messages from the system a joy.
5. Optional support for ponies.

The command for submitting a new message to the user could be named "usermessage", "amsg", "notify", "telluser" or something similar.

Keeping things simple and Arch-like is absolutely crucial.

Similar projects that I should look into first:
* https://github.com/Whonix/msgcollector
