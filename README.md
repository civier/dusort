
dusort
------

Run du with an admin user and sort the output. Everything is done within screen, so won't halt on network disconnection

Usage: dusort PATH [ USER FLAGS ]

PATH - path to tree that should be interogated
USER (optional) - user to switch to when executing the du command (if the current user is mentioned, no switch will be done)
FLAGS (optional) - flags to provide to du

Note: if wants to sort by level, might be easier to use tree --du, but difficult to know if it works, because it prints out the tree only when finished!
      dusort excludes files on other file systems

Author: Oren Civier

Acknowledgments: The author acknowledge the facilities and scientific and technical assistance of the National Imaging Facility, 
                 a National Collaborative Research Infrastructure Strategy (NCRIS) capability, at Swinburne Neuroimaging, Swinburne University.
