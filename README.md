# <img src="https://bampdx.com/wp-content/uploads/2015/12/BAMPDX-logo.png" height=28px width=45px>&nbsp;BAMsnap
<!--[![Build Status](https://travis-ci.org/bamsnap/bamsnap.svg?branch=develop)](https://travis-ci.org/bamsnap/bamsnap) 
[![Code Health](https://landscape.io/github/bamsnap/bamsnap/develop/landscape.svg?style=flat)](https://landscape.io/github/bamsnap/bamsnap/develop) 
[![Coverage Status](https://img.shields.io/codecov/c/github/bamsnap/bamsnap/develop.svg)](https://codecov.io/github/bamsnap/bamsnap?branch=develop)-->

## Installation

### Prerequisites
* python 3.0+
* [Pillow (Python Imaging Library)][pil] (5.0.0+)
* [pysam][ps] (1.8.1+)
* pyfasta

## Usage

### Simple usage
```bash
$ bamsnap -bam test.bam -pos 1:7364529 -out outpath
```

### Options
```
optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show program's version number and exit
  -bam [BAM [BAM ...]]  bam file
  -bamlist BAMLIST      list file with bam file paths
  -pos [POS [POS ...]]  genomic position (ex. 1:816687-818057, 12:7462545)
  -vcf VCF              list file with genomic positions with VCF format
  -bed BED              list file with genomic positions with BED format
  -out OUT              title of output file
  -out_type {png,jpg,html,image}
                        output file type
  -conf CONF            configuration file
  -ref REF              Reference sequence fasta file (ex. hg19.fa)
  -width WIDTH          image size : width (unit:px)
  -height HEIGHT        image size : height (unit:px)
  -read_thickness READ_THICKNESS
                        read width (unit:px)
  -read_gap_h READ_GAP_H
                        read gap height (unit:px)
  -read_gap_w READ_GAP_W
                        read gap width (unit:px)
  -draw DRAW            plot (default: -draw coverage,heatmap,read )
  -margin MARGIN        genomic margin size
  -center_line CENTER_LINE
                        draw center line
  -no_target_line NO_TARGET_LINE
                        do not draw target line
  -coverage_height COVERAGE_HEIGHT
                        coverage plot height
  -coverage_vaf COVERAGE_VAF
                        coverage variant allele fraction threshold (unit:%)
  -heatmap_height HEATMAP_HEIGHT
                        coverage heatmap height
  -draw_gene DRAW_GENE  draw gene structure
  -merged_image MERGED_IMAGE
                        draw a merged plot
  -colormap COLORMAP    colormap file
  -silence              don't print any log.
  -debug                turn on the debugging mode
```


### Examples

```
$ bamsnap -bam data/test11.bam -pos 1:715348 -out test/ex1
```
<img src="https://bampdx.com/wp-content/uploads/2015/12/BAMPDX-logo.png" height=28px width=45px>



