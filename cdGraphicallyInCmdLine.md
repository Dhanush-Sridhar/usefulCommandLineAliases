# **cd Graphically in cmdline**
## Graphically change Directory in cmd line
## Using ranger graphical comand file directory navigatory  
## Prequistis  
    - ranger 


```
    rcd(){
    # navigate and write to temp file 
    ranger --choosedir=OUTPUTFILE
    # copy the path saved in OUTPUTFILE to a temp variable 
    DIR=$( cat OUTPUTFILE )

    #remove file (do not liter your filesystem)
    rm OUTPUTFILE

    # change directory
    cd $DIR


```