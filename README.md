
This is yawei's unix assignment
In this assignment, there are two data files for me to inspect and analysis.
My UNIX assignment consists two components:
The inspection of data
The processing of these same data files to produce output files that are formatted for a subsequent analysis
My workflow for both data inspection and processing are as following:

#total 6209

#-rw-r--r--. 1 yaweil domain users       82 Sep 22 14:51 README.md

 #the number of column of fang_et_al_genotypes.txt 986
#  the number of column of snp_position.txt 15
#UNIX Assignment

##Data Inspection

###Attributes of fang_et_al_genotypes

here is my snippet of code used for data inspection
$wc

By inspecting this file I learned that:

the numbers of lines words bytes filename are 2783  2744038 11051939 respectively.
#$-rw-r--r--. 1 yaweil domain users 11051939 Sep 13 13:38 fang_et_al_genotypes.txt

###Attributes of snp_position.txt

here is my snippet of code used for data inspection
$wc 

By inspecting this file I learned that:

the numbers of lines words bytes filename are 984 13198 82763

#-rw-r--r--. 1 yaweil domain users    82763 Sep 13 13:38 snp_position.txt
##Data Processing

# $ awk -f transpose.awk fang_et_al_genotypes.txt > transposed_genotypes.txt # transpose file of fang

###Maize Data

here is my snippet of code used for data processing
Here is my brief description of what this code does

###Teosinte Data

here is my snippet of code used for data processing
Here is my brief description of what this code does
$ sed -i '1,3d' maize_transposed_genotypes.txt teosinte_transposed_genotypes.txt #delete Sample_ID, JG_OTU, and Group lines

$ sed '1d' snp_position.txt > snp_position_nohead.txt #delete head of snp

$ sort -k1,1V snp_position_nohead.txt > snp_position_nohead_sorted.txt

$ sort -k1,1V maize_transposed_genotypes.txt > maize_transposed_genotypes_sorted.txt #sort maize $ sort -k1,1V teosinte_transposed_genotypes.txt > teosinte_transposed_genotypes_sorted.txt #sort teosinte

$ join -1 1 -2 1 -t $'\t' snp_position_nohead_sorted.txt maize_transposed_genotypes_sorted.txt > maize_transposed_genotypes_joined.bed #join snp with maize

$ join -1 1 -2 1 -t $'\t' snp_position_nohead_sorted.txt teosinte_transposed_genotypes_sorted.txt > teosinte_transposed_genotypes_joined.bed #join snp with teosinte

$ sort -k3,3 teosinte_transposed_genotypes_joined.bed > teosinte_transposed_genotypes_joined_chr.bed #sort chrom colum

$ grep -v "^#" teosinte_transposed_genotypes_joined_chr.bed | cut -f3 | uniq -c #count chro
---output--- 155 1 53 10 127 2 107 3 91 4 122 5 76 6 97 7 62 8 60 9 6 multiple 27 unknown

$ sed -n '1,155p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr1.bed #chrom1 $ sed -n '156,208p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr10.bed $ sed -n '209,335p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr2.bed $ sed -n '336,442p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr3.bed $ sed -n '443,533p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr4.bed $ sed -n '534,655p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr5.bed $ sed -n '656,731p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr6.bed $ sed -n '732,828p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr7.bed $ sed -n '829,890p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr8.bed $ sed -n '891,950p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_chr9.bed $ sed -n '951,956p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_mutiple.bed $ sed -n '957,983p' teosinte_transposed_genotypes_joined_chr.bed > teosinte_transposed_genotypes_joined_unknown.bed

$ sort -k4,4V teosinte_transposed_genotypes_joined_chr9.bed > teosinte_chr9_ordered_increased.bed #ordered based on increasing position values and with missing data encoded by this symbol: ? $ sort -k4,4V teosinte_transposed_genotypes_joined_chr8.bed > teosinte_chr8_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr7.bed > teosinte_chr7_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr6.bed > teosinte_chr6_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr5.bed > teosinte_chr5_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr4.bed > teosinte_chr4_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr3.bed > teosinte_chr3_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr2.bed > teosinte_chr2_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr1.bed > teosinte_chr1_ordered_increased.bed $ sort -k4,4V teosinte_transposed_genotypes_joined_chr10.bed > teosinte_chr10_ordered_increased.bed

$ sort -k4,4nr teosinte_transposed_genotypes_joined_chr8.bed > teosinte_chr8_ordered_decreased.bed #sort decreased

$ sed 's/?/-/g' teosinte_chr8_ordered_decreased.bed #decreasing position values and with missing data encoded by this symbol: -

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr1.bed | sort -k4,4nr > teosinte_chr1_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr2.bed | sort -k4,4nr > teosinte_chr2_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr3.bed | sort -k4,4nr > teosinte_chr3_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr4.bed | sort -k4,4nr > teosinte_chr4_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr5.bed | sort -k4,4nr > teosinte_chr5_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr6.bed | sort -k4,4nr > teosinte_chr6_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr7.bed | sort -k4,4nr > teosinte_chr7_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr9.bed | sort -k4,4nr > teosinte_chr9_ordered_decreased.bed

$ sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr10.bed | sort -k4,4nr > teosinte_chr10_ordered_decreased.bed

sed 's/?/-/g' teosinte_transposed_genotypes_joined_chr10.bed | sort -k4,4nr > /home/yaweil/yawei-UNIX-Assignment/Data-Processing/teosinte_chr10_ordered_decreased.bed

/home/yaweil/yawei-UNIX-Assignment/Data-Processing
