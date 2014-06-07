NSE Bhavcopy Data

These files were downloaded from the NSE India website using the below command (change year as needed)

 for i in JAN FEB MAR APR MAY JUN JUL AUG SEP OCT NOV DEC; do x=${i}2007bhav.csv.zip;  for j in {01..31}; do wget -q --user-agent="Links (2.6; Linux 3.2.0-38-generic x86_64; GNU C 4.6.3; text)" http://www.nseindia.com/content/historical/EQUITIES/2007/$i/cm$j$x ; if [ -e cm$j$x ] ; then echo cm$j$x ; unzip -q cm$j$x ; rm cm$j$x ; fi ; done; done

These are archived here to make it easier to access for anyone that needs NSE EOD data.
