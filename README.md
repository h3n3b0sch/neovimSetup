# neovimSetup
### My neovim settings.

#### I installed neovim from source on a vanilla debian bookworm:  

Install the requirements:  
```sudo apt install build-essential```  
```sudo apt-get install ninja-build gettext cmake unzip curl```  
Install git:  
```sudo apt install git```  
Clone the neovim repository:  
```git clone https://github.com/neovim/neovim```  
Change directory into neovim and build:  
```cd neovim && make CMAKE_BUILD_TYPE=RelWithDebInfo```  
Make a package from the build and install the package:  
```cd build && cpack -G DEB && sudo dpkg -i nvim-linux64.deb```  
Make nvim the default editor:  
```sudo update-alternatives --install /usr/bin/vi vi /usr/bin/nvim 60```  
```sudo update-alternatives --install /usr/bin/vim vim /usr/bin/nvim 60```  
```sudo update-alternatives --install /usr/bin/editor editor /usr/bin/nvim 60```  
#### Setup neovim:  
Setting up neovim with references from different places:  
https://github.com/ThePrimeagen/init.lua  
