
to generate the binarized csv files 

1. make sure you have java on your machine and then change your directory to the directory of the mpd-binarizer.jar 

2.copy the datasets to the current directory

3.open terminal and type

java -jar mpd-binarizer.jar -k <lookahead days> -r<lookback days> -i <datset file name> -cat <up or down>

.
for example
java -jar mpd-binarizer.jar -cat up -i ArtistDatePlaysMatrixGT60sTop1K.csv -k 5 -r 50


The program will create a directory named by song_bin_of_ArtistDatePlaysMatrixGT60sTop1K.csv or something similary according to the input file name and each .moses files in the directory are named by each song Id in the original dataset.


Caution
=======

Please don't delete the lib folder and make sure the jar file and the lib folder always stay side by side


