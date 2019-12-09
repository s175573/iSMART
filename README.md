#immuno-Similarity Measurement by Aligning Receptors of T cells: iSMART

iSMART performs a specially parameterized pairwise local alignment on T cell receptor CDR3 sequences to group them into antigen-specific clusters. iSMART is developed by Bo Li (bo.li@utsouthwestern.edu), with all rights reserved. iSMART is under GPL3.0 license.

iSMART is written in Python2, and is portable without installations.

To use iSMART, please put all the downloaded files into the same directory with the source code, and use the command line to run:

'''
python iSMARTvx.py -f TCR_file ## Single file with variable gene

python iSMARTvx.py -f TCR_file -v ## Single file without variable gene

python iSMARTvx.py -d TCR_directory ## All files in a directory with variable gene. In this mode, after iSMART analyzes individual files, it performs cross comparisons between the CDR3 clusters identified from different individuals, and create a master table of shared CDR3s.
'''
Input file format:

CDR3 amino acid sequence (Starting from C, ending with the first F/L in motif [FL]G.G)

Variable gene name in Imgt format: TRBVXX-XX*XX

Joining gene name (optional)

Frequency (optional)

Other information (optional)
