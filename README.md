# Linux part II

## Prerequisite:
1. Connect to server (`ssh`)
2. Basic Linux command and getting help (`pwd`, `ls`, `ln`, `cd`, `cp`, `scp`, `mv`, `mkdir`, `rm`, `wget`, `git clone`, `du`, `df`)

## Topics will be covered
- using blast as example
    - Blast [hands-on](https://github.com/enormandeau/ncbi_blast_tutorial)

1. Download (`wget`, `git clone`) and Execute ([decompress](http://note.drx.tw/2008/04/command.html), install) program
    - download and decompress ncbi-blast-2.9.0+-x64-linux.tar.gz (ftp://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST)

2. Read (`cat`, `head`, `tail`, `more`, `less`, `wc`, `diff`) and edit (`touch`, `nano`, `vim`) file
    - git clone the repo for example file (https://github.com/enormandeau/ncbi_blast_tutorial.git)
    - fasta format: 2 lines per sequence
        1. header
        2. sequence
    - line counts (hint: using wc)
    - vim tutorial: (hint: using vim command mode)
        1. change all `reference_` to `ref-` in reference.fasta
        2. makeblastdb and blastn (practice with ln)

3. Advanced file edit (`grep`, `cut`, `sed`, `awk`, `join`, `paste`, `sort`, `uniq`)
    - download test vcf file (wget https://goo.gl/z1TBu9 -O test.vcf)
    - vcf format (at least 9 column)
    - line counts of headers (hint: using wc and grep)
    - awk, paste
    - categories counts of col7 (hint: using cut, sort, uniq)

4. (optinal) Docker
    - run a linux base container
    - build your own docker image with interactive mode
    - build your own docker image with Dockerfile
    - run your docker image
    - manage multi-images with docker-compose


## Assignment
1. Download and install `samtools`, then build index for reference.fasta
2. - report line counts of `col1 = chr1 and col2 between 10000 ~ 20000 (including 10000 and 20000) and col3 != .` in test.vcf (see Topics3), and write column 1, 2, 4, 5 to new.vcf
3. upload to server (ask shanghung in slack for more detail)


## Reference
1. https://github.com/WebbYang/Hello-World-Linux/edit/master/README.md (from 文策)
