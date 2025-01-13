Every block of sofware can be part of a sculpture larger than itself, it is the ambition of the curios collective to discover it.

Ranom findings in my Zig and computing machines journey got me thinking, and wanting to document some, here follows some of it...

# Zig, Rust and Go

The simplicity of Golang, its no nonsense aproach resonantes with my minimalistic core. Zig offers some awesome usability ( like self build) / utitlity (like c inerop) / features. But... these can also be found in golang.

In addition the golang stability, backward compatibility, package system, build speed, testability, no hidden control flow, to name a few have been very refreshing. All software languages exist for a reason, and as such are useful. 

I'm mostly working with enterprise systems and integrations, here my need is simple and fast which does not get in your way of solving business problems.

# To heap is human, to stack is divine

However when using Golang for ultra performance mission critical systems a recuring sticky point seems to be memory safety and allocation, there are some good blogs out there which demonstrate aproaches to optimise the GC overhead.

# Memory Safety What?

So what is memory safety? Is a GC language memory safe? What is the drive to memory safe languages? Security vaulnerabilities and failure modes. NSA objective 
buffer overwrites possible with GC ? It seems obvious, analyse the security flaws and for each determine how the system was compromised. or failure mode.

experience in systems programming for tiny spaces it seemed natural to consider the hardware, like clock cycles, memory use and allocations and so on. Then came a time where mortals had no longer to concern themsels with such low level detail, until we had to go faster. Yet safe, and repeatable.

https://tip.golang.org/doc/gc-guide

Can a different GC strategy be used to improve performance?

https://github.com/tinygo-org/tinygo
Here I tried to compile gitlab.com/cznic/sqlite with tinygo, bur found runtime.Pinning not implemented.

The new arena language feature:

https://pyroscope.io/blog/go-1-20-memory-arenas/

https://go.dev/wiki/Performance

Memory safety can there be an extension to fix this? Does it need fixing, is go memory safe?
