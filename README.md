# NSX-Create-Security-Group-Tags
A script to create NSX-v Security Groups and associated Security Tags as dynamic members

##Prerequisites
Requires the Requests libraby to be installed. Requests can be downloaded a from the following URL
http://docs.python-requests.org/en/latest/

##Usage
```
python nsx-create-sg-tag.py -h
```
Output:
```
usage: nsx-create-sg-tags.py [-h] [-u [user]] -s nsxmgr -i inputfile [-d]

Create NSX-v security security tags from CSV file and add them to the
associated Security Group.

optional arguments:
  -h, --help    show this help message and exit
  -u [user]     OPTIONAL - NSX Manager username (default: admin)
  -s nsxmgr     NSX Manager hostname, FQDN or IP address
  -i inputfile  Input file in csv format
  -d            Enable script debugging
```
##Example
An example to run the script
```
python nsx-create-sg-tags.pyy -s nsxmgr-l-01a.corp.local -i inputfile.csv
```
