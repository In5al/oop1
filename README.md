#Full Instalation
##Setting Ubuntu
>Firstly I chose to dual-boot so I reservered 100GB for Ubuntu. At partion more than 10 went so swap memeory while the rest as root.a]After all was set up,i made the necesary upgrades and necesary updates via "sudo apt update" and "sudo apr upgarde". Aditionally I set a new browser as the default one and of course Discord.
##Changing from bash to zsh 
>Firsly I had to install several commands like vim and chsh by using "sudo apt install".What followed was instaling zsh using the same procedure "sud apt install" and then changing from bash to zsh.Then we ran zsh and configured 2 of the mutiple settings.'Continue to main-menu(1)'-->Configure settings(1),then activating the 3 settings(1)(2)(3).Then we save and exit (0). By command "echo $SHELL" we check the curent shell. As following the steps the curent shell would still be bash. Next by using commands "chsh -s/bin/zsh aeon" . I changed the shell on local user . After that, by using "chsh -s bin/zsh root" I changed the shell for root user as well.All thats left is to restart the PC.
##Installing oh-my-zsh
>As we did when installing zsh we had to instal some programs an as the other oenn the first one requiring was curl and did by usinf "sudo apt install". After it we ran thr command "curl -L http://install.ohmyz.sh | sh" And we were done.After closing and reopening the terminal the terminal interface changed.
##Customizing oh-my-zsh
>By using command "ls -la" we found the file ".zshrc".Using command "vim .zsh" Which is a substitute text editor to neno we enter in "oh-my-zsh". Here we can change a ot of stuff but I chose to change the backgrounf to Cypher and to save the changes which gave me a little bit of trouble the following commands weew necesary "ESC-:wq!"
##Installing gcc
>The necesarry files (gcc, g++..) are all installed by the command "sudo apt install built-essential". THen we can check the version of gc (gcc --version) 
##Creating first C file using gcc and other commands
First we choose a directory and a place for our C file. By using "ls" to see our current location by listing the files liocated in that directory we chose to go in or out of a directory by using the command "cd". To exit/go back we use "cd.." and to enter/move in we use "cd___"and we place the chosen directory.
I chose to place my c file on Desktop. To create a file we use the command "touch__" and the desired name. I chose "touch test.c"And so a test.c was created. By using a text editor like "subl test.c" or doning it out of terminal we write our C code.By commands "gcc hello.c -o test" We run and the aditional "-o test" would create a binary file which is the output file of the code we wrote in test.c. Using "./test" we run the output file 
##Installing SublineText as the text editor 
>Folowing the steps given on their official website we install SublineText taking into consideration the Linux Distribution we have installed. First we install the GPG key"wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/sublimehq-archive.gpg". Next we chose a chanel from which we choose to install subline text. I chose the stable one:"echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list".
Next we install subline-text using the command "sudo apt-get install sublime-text". Finally we make sure that the apt is configured to work with https sources:"sudo apt-get install apt-transport-https"
##Installing and configuring git 


