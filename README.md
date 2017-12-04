
= mass googler =

Google a large collection of subjects as listed in a text file. The searches can be modified. For very large searches, a sub-set of searches can be run at a time. 


== usage ==

    massgoogler -i search_terms.txt 
                             [--search=classic|vintages [--search=...] ]
                             [--lucky]
                             [--lucky-plus ]
                             [--start    12]
                             [--rows     30]
                             [--sleepSec  1]
    
    massgoogler -i website_addrs.txt 
                             [--massOpen   ]
                             [--prepend = "www."]
                             [--dupPrepend = "www."]
                             [--start    12]
                             [--rows     30]
                             [--sleepSec  1]
							 

where:

   -i              the file listing the search terms, one per line
   [--search=...]  a string to add to the search page
   [--lucky]       forward to the "I feel lucky" page 
   [--lucky-plus]  forward to the "I feel lucky" page AND show google search
   [--massOpen]   just open the web addresses (NO google search)
   [--start n]     start on the nth non-comment, non-empty row [default=1]
   [--rows n]      how many non-comment, non-empty rows to process [all]
   [--sleepSec n]  how many seconds to sleep between searches [1]
   [--prepend = "www."]      prepend "xxxx" to each web address (only)
   [--dupprepend = "www."]   prepend "xxxx" to each web address, and do orig addr


	
Currently, for this simple program to work properly:
* 	firefox/iceweasel must be already running, and
* 	for --lucky to work: set google to settings > 'never show instant results'
*   google no longer supports "I'm Feeling Lucky" 


== prerequiesite ==

This simple program uses firefox, so it has to be installed. Yes, there are more sophisticated solutions. Uses a few Perl libraries that most any installation should have. 




