# FixedWidthToDelimited

This script will convert Fixed width File into Delimiter File, tested on Python 3.5 using Windows Subsytem for Linux (WSL)

Sample run: (Order of argument doesnt matter)

go to the directory containing this .py files
cd /mnt/c/yourpathfolder

run the command in WSL
./python3 FixedWidthToDelimiter.py -i SrcFile.txt -o TrgFile.csv -c Config.txt -d ","

Inputs are as follows

1. Input FIle - Mandatory(Argument -i) - File which has fixed Width data in it
    use .dst or .pdb files generated from the chemo/bioinformatics program
    
2. Config File - Optional (Argument -c, if not provided will look for Config.txt file on same path, if not present script will not run)
    For each column, format as following, example for dividing .dst file into columns
    FieldName,fieldLength
    eg:
    x1,6
    x2,5
    x3,16
    x4,32
    x5,12
    x6,8

3. Output File - Optional (Argument -o, if not provided will be used as InputFIleName plus Delimited.txt)

4. Delimiter - Optional (Argument -d, if not provided default value is "|" (pipe))

