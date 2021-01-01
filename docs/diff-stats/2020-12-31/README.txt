This contains the diff stats using the original data from the other third-party transcriptions.
It doesn't reflect any changes made to other transcriptions since the download of the 
original data from DPC, Wikisource, and Project Gutenberg, done in late November 2020.
(In practice, only Wikisource has changed since that time, but those changes haven't 
been brought into the project yet.)

Example command used:
git diff --stat --output=C:/temp5/diffs/2020-12-31/1908-LCP-4th-versus-1908-LCP-4th-corrected.txt  1908-LCP-4th 1908-LCP-4th-corrected -- "*.utf8"

Note how it filters-in the .utf8 files, to avoid comparing anything else.
git diff --stat --output=C:/temp5/blah.txt BranchA BranchB -- "*.utf8"

To see the diffs themselves, just leave out the --stat option. More info: 
https://git-scm.com/docs/git-diff

Example of full diff, with no preamble:
git diff --unified=0 --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-versus-1908-LCP-4th-corrected.txt  1908-LCP-4th 1908-LCP-4th-corrected -- "*.utf8"

Versus Raw 1908:
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-versus-1908-LCP-4th-corrected.txt  1908-LCP-4th 1908-LCP-4th-corrected -- "*.utf8"
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-versus-DIG-DPC-2008-05.txt  1908-LCP-4th DIG-DPC-2008-05 -- "*.utf8"
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-versus-DIG-GUT-0000.txt  1908-LCP-4th DIG-GUT-0000 -- "*.utf8"
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-versus-DIG-WIK-1908-11th.txt  1908-LCP-4th DIG-WIK-1908-11th -- "*.utf8"

Versus Corrected 1908:
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-corrected-versus-DIG-WIK-1908-11th.txt  1908-LCP-4th-corrected DIG-WIK-1908-11th -- "*.utf8"
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-corrected-versus-DIG-GUT-0000.txt  1908-LCP-4th-corrected DIG-GUT-0000 -- "*.utf8"
git diff --stat --output=C:/temp5/diffstats/2020-12-31/1908-LCP-4th-corrected-versus-DIG-DPC-2008-05.txt  1908-LCP-4th-corrected DIG-DPC-2008-05 -- "*.utf8"
