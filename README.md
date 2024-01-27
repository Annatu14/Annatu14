### Usage and more information
## how to run your setup.sh script
## open your terminal and add the following prompts in the command line(press enter to execute a prompt)
nano setup.sh
## once this is executed, a text editor is opened where these instructions will be inputed.

# we will make a directory to hold the data, download the data
# and uncompress it

echo "making directory"
mkdir HCEPDB
cd HCEPDB

echo "making README"
echo "This directory holds a copy of the HCE PDB" > README.txt

echo "downloading data"
curl -O http://faculty.washington.edu/dacb/HCEPDB_moldata.zip

echo "uncompressing zip"
unzip -x HCEPDB_moldata.zip

echo "here are the first two lines of the csv file"
head -2 HCEPDB_moldata.csv

echo "removing zip file"
rm HCEPDB_moldata.zip
## once this is done, press "control +X" on your keyboard to exit
## you will be prompted to "Save modified buffer?", press 'y' on your keyboard to save it 
## click enter to go back to your command line
## start to type this commands
cat setup.sh
## this should print out the same instructions in your setup.sh
sh setup.sh
## this will execute the commands in your setup.sh 
## you should also be able to see the downloading proceess after which you see the rest of the commands being executed
 % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  168M  100  168M    0     0  20.6M      0  0:00:08  0:00:08 --:--:-- 20.1M 

## this is how to run the setup.sh



