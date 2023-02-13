- ## wsl
	- ### uninstall ubuntu from wsl2
	  wsl --uregistered Ubuntu
	  winget  uninstall Ubuntu
	  winget uninstall -id Canonical.ubuntu
	- ### export 
	  run windows system32 terminal as admin
	  wsl --export Ubuntu D:\ubuntu\ubuntu.tar
	  wsl --import <distro name> D:\ubuntu\ D:\ubuntu\ubuntu.tar
- ## open virtual env for python
	- activate python first inside wsl ubuntu 
	  python -m venv venv
	  source venve/bin/activate
	- start vscode 
	  code .
	- Go to any folder 
	  open any python file or project 
	  open tmc then open work space
	- Wait for Ubuntu to recognize python and virtual env