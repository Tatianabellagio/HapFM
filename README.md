# HapFM

HapFM has 2 main functions: genome-wide haplotype block partition and haplotype-based fine-mapping.

## Usage

### Prerequisite

Python3: modules including numpy,scipy,pandas,networkx,pyclustering and sklearn

R: gpart and optparse 

(Note that gpart requires /lib64/libstdc++.so.6: version `GLIBCXX_3.4.20', try a older version of gcc)

### Haplotype block partition and cluster formation
python3 bin/HapFM_haplotype.py -v VCF -b bigld -o output

The output file (haplotypeDM) will become the input of the haplotype-based fine-mapping step.

### Haplotype-based fine-mapping
python3 bin/HapFM_mapping.py -i haplotypeDM -c covariates -y phenotype -o output




