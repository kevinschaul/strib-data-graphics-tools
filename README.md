# Star Tribune web dev tools installation

## Must-haves

### [Xcode](https://developer.apple.com/technologies/tools/)
Includes tools needed to compile software

Via the Mac App Store

Note: An [Apple developer account](https://developer.apple.com/register/index.action) is required.

1. Open Xcode
2. Agree to license
3. Open preferences
4. Downloads tab
5. Download/install "Command Line Tools"

### [homebrew](http://brew.sh/)
Package manager for OS X. Helpful for installing other software

    su schaullocaladmin        # User with admin privileges
    ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"

    # From regular account:
    brew doctor

    # Fix any issues. To fix mine, I ran:
    su schaullocaladmin
    sudo chown -R schauka /usr/local

### [git](http://git-scm.com/)
Version control

    brew install git

    git config --global user.name 'YOUR NAME'
    git config --global user.email 'YOUR@EMAIL.com'
    git config --global push.default matching

    # For `git st` shortcut
    git config --global alias.st 'status -s -b'
    
    # For pretty colors
    git config --global color.ui true
    
    # If you want to use Sublime Text to edit your commit messages:
    ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
    git config --global core.editor 'subl -w'

I recommend using ssh authentication. [Here's how to set that up](https://help.github.com/articles/generating-ssh-keys)

### [node](http://nodejs.org)
JavaScript without a browser

    brew install node

### [grunt](http://gruntjs.com)
Project-level tasks for repetitive things

    npm install -g grunt-cli
    
### [homebrew-php](https://github.com/josegonzalez/homebrew-php)
Useful for previewing projects with Star Tribune includes

    brew tap homebrew/dupes
    brew tap josegonzalez/homebrew-php
    brew install php54

### [VirtualBox](https://www.virtualbox.org/)
Test your code in different environments

Via .pkg installer

### [ievms](https://github.com/xdissent/ievms)
Test in IE6, 7, 8, 9 and 10 using VirtualBox

Note: This downloads ~15GB of files.

    curl -s https://raw.github.com/xdissent/ievms/master/ievms.sh | bash

## Data analysis tools

### [csvkit](http://csvkit.readthedocs.org/en/latest/)
Command-line tools for manipulating/exploring .csv files

    sudo pip install csvkit

### [R Studio](http://www.rstudio.com/)
Statistical analysis, graphing software

Requires [R](http://www.r-project.org/)

Via [.dmg installer](http://www.rstudio.com/ide/download/)

### [qgis](http://qgis.org/en/site/)
GIS system

Requires [GDAL Complete](http://www.kyngchaos.com/software/frameworks#gdal_complete)

Via [.pkg installer](http://www.kyngchaos.com/software/qgis)

## Might be nice for future projects

### [gdal](http://www.gdal.org/)
Geospatial data library, command-line tools

    brew install gdal

### [pip](https://pypi.python.org/pypi/pip/)
Python package manager

    su schaullocaladmin        # User with admin privileges
    sudo easy_install pip

### [virtualenvwrapper](http://virtualenvwrapper.readthedocs.org/en/latest/index.html)
Project-level python package scope

    su schaullocaladmin        # User with admin privileges
    sudo pip install virtualenvwrapper

## Personal choices

### [macvim](https://code.google.com/p/macvim/)
Best text editor

    brew install macvim

### [janus](https://github.com/carlhuda/janus)
Helpful mods to vim

    curl -Lo- https://bit.ly/janus-bootstrap | bash

### [Google Chrome](http://google.com/chrome)
Browser

Via .dmg installer

### [Markdown Preview](https://chrome.google.com/webstore/detail/markdown-preview/jmchmkecamhbiokiopfpnfgbidieafmd?hl=en-US&utm_source=chrome-ntp-launcher)
Preview .md files

Via Chrome Web Store
Be sure to "Allow access to file URLs" in the settings

### [Dropbox](http://dropbox.com)
File syncing service

Via .dmg installer
### [LibreOffice](htpp://www.libreoffice.org)
Open source office applications

Via .dmg installer
