## Extra Linux Commands and Comments

### *SUDO*
` sudo !! ` will redo last cmd but as root 

### *AVOID HISTORY*
maintaining a *leading space* before a cmd on the cmd-line will keep it from being stored in **history**

### *TEE*
whilst `tee` writes **stdin** to a file *and* **stdout**, `tee -a` will *append* to the file and **stdout**

### *PING*
`ping` sends pockets of data (ICMP ECHO_REQUESTs) to specified IP address to test the ability of your computer to reach the specified destination
- use option *c* (count) then a # argument to specify how many requests are sent (ex. `ping -c 3`)

### *IN-TERMINAL PYTHON*
`python3` will run Python 3 in the terminal

### *MAKING PARENTS*
`mkdir -p` creates parent directories of pathway arguments
- for example: `mkdir -p direc/direc2/file1` will create direc with direc2 in it with file1 in direc2 (given they are uncreated)

### *TABS <-> SPACES*
`expand` converts all tabs in files to equivalent spaces
- `unexpand` does the opposite  
