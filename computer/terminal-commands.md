---
title: "Terminal commands"
output: 
  html_document:
  toc: true
  toc_float: true
---

## Common {.tabset}

### Mac

Command | Description
:----------------------------------------------- | :------------------------------------------------------------------
ls -la  | lists files, flags put in a list and show hidden files
open < *filename* \| . > | opens *filename* with the default application \| opens the current directory
touch *filename*   | stamps *filename* with current system file, but if *filename* does not exist it will be created
mkdir -p *dirname* | creates the folder *dirname* - the $-p$ flag ensures that any "parent" directories will also be created
rm *filename* | deletes *filename*
rm -i *filenames* | prompts whether to delete each file - requires interaction
rm -r *dirname* | deletes *dirname* and contents
rm -ri *dirname* | prompts whether to delete contents and *dirname* - requires interaction
rmdir *dirname* | remove **empty** directory *dirname*


### Windows

(tab content)

## Network {.tabset}

### Mac

Command | Description
:----------------- | :------------------------------------------------------------------
ifconfig en0 inet  | get local ip 
dig +noall +answer *URL*  | can be used to check DNS records of *URL* 


### Windows

(tab content)
