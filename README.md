# R_HTML_quality_report
Convert table of values to passing report for assay evaluation

The aim of this R script is for internal evaluation of new primer designs. We call each design/target as assay, made up of one forward and one reverse primer. We then combine these assays in a 4-plex reaction. Do these primers work together as a 4-plex and maintain specificity? That is the question. To fail means an assay needs to be reworked or dropped from the multiplex. The output from the experiment is a relative florescence intensity (RFI), such as the kind you might get from qPCR with limited cycles (not to plateau but to the inflection point, thus different for different template staring amounts)

What this script seeks to do it provide a summary report that a lab RA can read, check for pass or fail falgs. If all pass, they can proceed with the assay applied to real samples. If something fails, they can escalate that to a senior design person/manager and the report also will indicate which assay is failing, and in what respect (off-target, lower than expected abundance, etc.)

It is fast and dirty, but gets the job done.
