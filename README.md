# repro-tools
A set of tools to evaluate the reproducibility of computations.


## Getting Started

verifyFiles.py is a Python Script which will produce an output containging the details regarding the common files and files that are not common, based on timestamp, checksum and distance between the output files.

### Prerequisites

Python 2.7.5

## Running the script

```
usage:verifyFiles.py [-h] [-c CHECKSUMFILE] [-d FILEDIFF] [-m METRICSFILE] [-e EXCLUDEITEMS] [-k CHECKCORRUPTION] [-s SQLITEFILE] [-x EXECFILE] file_in

file_in,                                   Mandatory parameter.Directory path to the file containing the conditions.
-c,CHECKSUM FILE    --checksumFile         Reads checksum from files. Doesn't compute checksums locally if this parameter is set.
-d FILEDIFF,        --fileDiff             Writes the difference matrix into a file.
-m METRICSFILE,     --metricsFile          CSV file containing metrics definition. Every line contains 4 elements: metric_name,file_extension,command_to_run,output_file_name
-e EXCLUDEITEMS,    --excludeItems         The path to the file containing the folders and files that should be excluded from creating checksums.
-k CHECKCORRUPTION, --checkCorruption      The script verifies if any files are corrupted ,when this flag is set as true
-s SQLITEFILE,      --sqLiteFile           The path to the SQLITE file,having the reprozip trace details.
-x EXECFILE ,       --execFile             Writes the executable details to a file.
-b BINARY MATRIX,   --binaryMatrix         Shows the existence of difference between the conditions of the condition pair in terms of the subject and file.
-t TRACK PROCESSES  --trackProcesses       If this flag is set, it traces all the processes using reprozip to record the details and writes it into a csv with with the given name
```

### Test Cases

To be updated


## Authors

* **Big Data Lab Team - Concordia University**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details



