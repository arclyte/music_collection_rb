# music_collection_rb
Small ruby command line script to manage a music collection

To run: ./music

Supports functionality described here: https://gist.github.com/jgoulah/fc742e8512ff730a86d262c25bbf549b

I played around with unit testing the functions here using Ruby's built-in test library, but the code would require some 
refactoring for it to work properly.  As it sits now, it directly outputs (via print/puts) to stdout.  In order to allow 
testing I'd want to split off code as a separate class from the runner (`mc.run()`) and allow it to take commands directly
as well as user input on stdin (`gets`).  The MusicCollector class was purpose built to run this script, but this kind of
functionality would work best with a more generic 'CLI' library that provided utilities for output.
