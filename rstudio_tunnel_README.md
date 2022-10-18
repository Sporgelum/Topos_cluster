# How to create a tunnel through the cluster


*1. Download this script.

Wget https://gist.githubusercontent.com/pansapiens/b46071f99dcd1f374354c1687f7a986a/raw/rstudio.sh

*2. Download my script and set the `rstudio version` you want in the script.

“add git link”

*3. Select the `port you want` in the script.















*4. Create an interactive session(example).

`srun –mem-per-cpu=8 –ntasks-per-node=8 --nodes=1 --partition=pall --time=06:00:00 --pty bash`

*4.1. In my case after being allocated to the respective session I have `singularity` available to run, but might have to check in each system if shall be loaded or it is already available.

*4.2 Set the –server-user to your user if does not work.


*5. Set the script as executable 
`chmod +x ./rstudio.sh`

*6. Check `squeue -u ${USER}` for the session you are allocated and use `host session allocated` to know it.


*7. Run the script and shall download the version of R you want, run through the port selected and give you which link to paste and which to open, with the respective user and password.


*7.1. Use the pink arrow in a local console out of the cluster.

*8. Have by the side the `PASSWORD` of the cluster to use.
*9. User and Password for the browser link which I usually open in Chrome.
