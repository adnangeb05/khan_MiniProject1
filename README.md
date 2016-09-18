# khan_MiniProject1

##Miniproject1 BIOL797
Sept 19,2016

##Part1: 

Download the csv files in the linux (fedora). 

In the first part of the miniproject one the recorded file was downloaded and viewed using excel.

The directory and subdirectory were created for the two mouse species data file using `mkdir` command.

Copy them in the DOM and CAST directory according to the data type using cp commnad.

Later the files were observed in less using `less -S` command.


Part 2: For the CAST data:

Header command was used to save the first 10 lines for further use and  

Step 8.a

Original record file:

wc 0008659-160822134323880.csv 
  1676  64987 758379 0008659-160822134323880.csv

Uniq file :
wc CAST_lat_long_uniq.txt 
  1676  64987 758379 CAST_lat_long_uniq.txt

Percent of duplication: (1676-1676/1676)*100=0.0% duplication data.

Step 9

Original record file:

wc 0008659-160822134323880.csv 
  1676  64987 758379 0008659-160822134323880.csv


grep USNM file: 

wc CAST_USNM.txt 
  1317  50463 592045 CAST_USNM.txt

USNM collected data is (1317/1676)*100=78.58%

Step 10

wc CAST_USNM_lat_long.txt 
1317  158 3750 CAST_USNM_lat_long.txt

Commands used 

cd CAST/
   19  ls
   20  head 0008659-160822134323880.csv > CAST_header.txt
   21  nano 0008659-160822134323880.csv 
   22  wc 0008659-160822134323880.csv 
   23  sort -k17 -n 0008659-160822134323880.csv > CAST_sort_lat.txt
   24  ls
   25  uniq CAST_sort_lat.txt > CAST_lat_uniq.txt
   26  sort -k18 -n CAST_lat_uniq.txt > CAST_sort_lat_long.txt
   27  uniq CAST_sort_lat_long.txt > CAST__lat_long_uniq.txt
   28  wc 0008659-160822134323880.csv 
   29  ls
   30  uniq CAST_sort_lat_long.txt > CAST_lat_long_uniq.txt
   31  rm CAST__lat_long_uniq.txt 
   32  wc CAST_lat_long_uniq.txt 
   33  grep "USNM" 0008659-160822134323880.csv > CAST_USNM.txt
   34  wc CAST_USNM.txt 
   35  awk 'FS="\t" {print $17, $18}' CAST_USNM.txt > CAST_USNM_lat_long.txt
   36  wc CAST_USNM_lat_long.txt 
   37  less -S CAST_USNM_lat_long.txt 
   38  grep -v “^\s*$” CAST_USNM_lat_long.txt > CAST_lat_long_cleaned.txt
   39  nano CAST_lat_long_cleaned.txt 

For the DOM data:

Step 8.a

Original record file:

wc 0008658-160822134323880.csv 
   8481  388042 4210761 0008658-160822134323880.csv

Uniq file :
wc DOM_lat_long_uniq.txt 
   8389  382961 4156828 DOM_lat_long_uniq.txt

Percent of duplication: (8481-8389/8481)*100=1.085% duplication data.

Step 9

Original record file:

wc 0008658-160822134323880.csv 
   8481  388042 4210761 0008658-160822134323880.csv


grep USNM file: 

wc DOM_USNM.txt 
   4346  180057 2009855 DOM_USNM.txt

USNM collected data is (4346/8481)*100=51.24%

Step 10

wc DOM_USNM_lat_long.txt 
 4346   594 11733 DOM_USNM_lat_long.txt

Commands used:

Part 3: 









