bamWindow
===========
bam-window reports the number of reads mapping within adjacent windows on the genome.
It reports the number of reads overlapping the window or optionally, just reports the
number whose leftmost mapping coordinate is within the window. Use -d to report only a
random sampling of the reads within the window. This is useful for approximating results
at lower coverage depths.

Usage
-----

Version 0.4
Usage: bam-window <bam_file>

    -q INT    filtering reads with mapping quality less than INT [0]
    -w INT    window size to count reads within [1000]
    -p        only include paired reads
    -P        only include properly paired reads
    -s        only count a read as in the window if its leftmost
              mapping position is within the window
    -l        output a column for each library in each window
    -r        output a column for each read length in each window
    -d FLOAT  probability of reporting a read [1.000000]

bam-window reports the number of reads mapping within adjacent windows on the genome.
It reports the number of reads overlapping the window or optionally, just reports the
number whose leftmost mapping coordinate is within the window. Use -d to report only a
random sampling of the reads within the window. This is useful for approximating results
at lower coverage depths.

    The -l option creates separate counts for each library
    The -r option creates separate counts for each read length
    The -l option can be paired with the -r option to get separate counts for each read length


xxx

