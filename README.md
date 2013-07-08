phraug
======

A set of simple Python scripts for pre-processing large files, things like splitting and format conversion.

See [http://fastml.com/processing-large-files-line-by-line/](http://fastml.com/processing-large-files-line-by-line/) for the basic idea.

`count.py <input file>`

Count lines in a file. On Unix you can do it with `wc -l`

`csv2libsvm.py <input file> <output file> [<label index = 0> <skip headers = 0>]`

Convert CSV to LIBSVM format. If there are no labels in the input file, specify <label index> = -1. If there are headers in the input file, specify <skip headers> = 1.

`csv2vw.py <input file> <output file> [<label index = 0> <skip headers = 0>]`

Convert CSV to VW format. Arguments as above.

`libsvm2csv.py <input file> <output file> <input file dimensionality>`

Convert LIBSVM to CSV. You need to specify dimensionality, that is a number of columns (not counting a label).

`libsvm2vw.py <input file> <output file>`

Convert LIBSVM to VW.

`split.py <input file> <output file 1> <output file 2> [<P: probability of writing to the first file>] [<random seed>]`

Split a file into two randomly. Default P is 0.9. You can specify any string as a seed for random number generator.

`subset.py <input file> <output file> [<offset = 0> <lines = 100>]`

Save a subset of lines from an input file to an output file. Start at <offset> (default 0), save <lines> (default 100).
	
	
	