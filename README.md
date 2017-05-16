# pdfsmaller
This is a basic version that works for local files to reduce PDF file
size.

The script moves through subfolders sending each PDF file to
ghostscript to reduce size.

This version uses the ‘default’ ghostscript setting. Change to ‘screen’
for more aggressive file size reductions.

Its possible that some of the files output will be larger than the
original file. Also that output files will have unacceptable reductions
in quality in some cases. For this reason, the original files are not
replaced, they are stored at the output path.

Spaces in destination filenames are replaced with underscores at line 18

After running the script, the next step would be running a file that
compares the original and optimised files to report on overall file
size reduction.

This would be followed by a script to replace original files with the
optimised files where the optimised file is smaller. This approach
assumes that you can live with any possible reduction in quality.
