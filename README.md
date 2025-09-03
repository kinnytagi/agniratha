this is an untitled programming language based on the minecraft create mod's 6.0.0 factory processing update.

yes that is entirely so nerdy but i really don't care.

consider this language to be a frankenstein of the functional and object oriented styles. 

(i am making the names up as i go (for later revision))
at its core, there are two basic items you work with: vaults and tickers.

vaults are external files that the language stores all of its data in / gets all of its data from.

tickers are sets of instructions that act on the data stored in those vaults. 

tickers, however, can only move this data to different places in the language's network.
it's at the network's destinations (which are vaults) that can do operations on this data.

in a way, this is similar to a processor's methods of calculation.
data is moved to certain chips in the computer, which then perform logical operations
on that data.

consider addition. data from the processor's registers is moved to the ALU, which
then performs addition on the data moved to it, and the output is moved to some
meaningful location for the programmer.

my language works in the same way. a ticker calls for data to be moved from a vault
to some other vault that's designed to do something with its intake, and the ticker
then moves the result to some meaninful place, possibly the vault for output (stdout).

each vault has a link and packager embedded into it. the link allows for a ticker to
interact with a vault and order its data to be moved through the network (the network
being the composite of all tickers and vaults involved witha  program). the packager
is simply a port for data to move through. 

within the packager, the protocol for input and output can be changed, allowing for
computation and logic upon the arrival or departure of data.

a new idea: promises. an expression can be defined as a promise that it will eventually contain data. this is useful for situations like user input. the object exists, which means that data isn't being created during runtime, but it can be variable, which makes the language interactive.
