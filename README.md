bash-session
============

Sessions for bash. One of the few things that still drives me crazy on with computers is losing my working context due to system crashes or power failures. I hope to relieve this pain with some bash 'magic'.

Goals
=====

The in end, I would like to have:
 - a persistant contextual history of commands issued into the shell for later reference
 - a grouping mechanism/identification scheme for external session containers
 - the ability to recover as much context/session as possible after a crash, such as:
  - environment varibles with configureable white-/blacklists
  - current working directory and directory stack
  - the local history of the shell in the order the commands were entered not interleaved with commands entered in other sessions
  - positions and groupings within external session containers (like screen, tmux, terminator and the likes)
  - redirections that are in effect (though this might legitematly not be possible)
  - open files (see above)
 - commands/functions for managing these sessions
  - create
  - copy
  - rename
  - delete
  - move between session groups
  - inspecting sessions (e.g. like searching in the history)
 - the persistance format should be reasonably human readable, or be easily converted into a human readable form
 - should have little, better yet no external depedancies, for maximum portability (idealy only bash and posix tools as hard dependancy)
 - should scale properly over time. Not get ever slower the longer the history gets
 - should have reasonable memory footprint
 - should play along nicely with version control and unison/rsync

