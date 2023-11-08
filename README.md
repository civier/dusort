

   dusort
   ------
   Run du in a detached terminal (i.e. resister to network disruptions) and sort the output.

    Usage: dusort PATH [ USER FLAGS ]

     PATH - path to tree that should be interogated
     USER (optional) - user to switch to when executing the du command (if the current user is mentioned, no switch will be done)
     FLAGS (optional) - flags to provide to du (e.g., '--inodes' indicates to count number of files rather than calculate volume)

    Note: * dusort prints error code. If error code is non-zero, run 'grep ^du: LOGFILE.txt' to display the the error messages.
          * dusort excludes files on other file systems
          * to sort by level in the hierarchy, might be easier to use tree --du, but beware that errors, if any (e.g., unaccessible files), will only be evident when the command finishes executing. 
	     Unfortunately, 'tree --du' does not provide any feedback throughout execution.

    Author: Oren Civier

    Acknowledgments: The author acknowledge the facilities and scientific and technical assistance of the National Imaging Facility, 
                     a National Collaborative Research Infrastructure Strategy (NCRIS) capability, at Swinburne Neuroimaging, Swinburne University.


