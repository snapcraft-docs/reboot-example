# Example reboot snap

This project shows how a snap can be used to reboot a system.

See this forum message for the original implementation and context:
https://forum.snapcraft.io/t/strict-confined-snap-system-reboot-how-to-w-python/26033/2

Note that the snap's `shutdown` interface needs to be manually connected from
outside the snap since this interface is not auto-connected by default.
This can be done by running `sudo snap connect reboot-example:shutdown` in a
terminal.

Obviously, this limits the usefulness of the snap, but it may be useful for
some purposes.
