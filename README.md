![GA_Logo](https://raw.github.com/generalassembly/ga-ruby-on-rails-for-devs/master/images/ga.png)

#WDI Installfest 


We are going to install the tools necessarily to program with Ruby and Rails on your computer.

If you are unsure or run into problems during installation, don't worry; We will finish up any of the loose ends on Installfest.
	

##Verify your install
If you have already experimented with ruby or rails before, verify your versions are correct for this upcoming class.

If you can see the correct version numbers when you run the commands in Terminal below, you are good to go.

**Verify you are running 2.0 of ruby**

`ruby -v`

**Verify you are running version 4 of Rails**

`rails -v`

If not, continue with the instructions to get your envionment going. Run these again after you're done to ensure everything is working properly.

---
---


#Mac Instructions
* Install Xcode or Command Line Tools
* Install Homebrew (Software Package Manager for Mac)
* Install GIT
* Install RVM and Rails
	

##Install Command Line Tools
If you are running Maverick, you don't have to install Xcode in order to get command line tools.

In your terminal type `xcode-select --install` and a new window and installer will appear. 


##Xcode
If you are not running Maverick, you will need to install Command Line tools that come from Xcode.


*	Create an account on Mac App Store if you haven't already.
*	Upgrade your OS to the latest version possible using the Mac App Store (Maverick is the latest version) - The cost of Mountain Lion is around $20, most people will already have it, but if you can upgrade, you should!
*	Open the Mac App Store and install Xcode
*	Open Xcode, Choose Preferences, Downloads and then Install The Command Line Tools




##Install Homebrew

###Homebrew
[http://brew.sh/](http://brew.sh/)

Homebrew is a package manager, a program which will install other programs that we need.  Open up the application Terminal and run the command below to install Homebrew

```
ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
```

![image](./install_brew.png)

###Brew Doctor
Run brew doctor in your Terminal to let you know if the install was successful. It will give you tips on what you can do to corrrect any system wide issues. If you do have any problems, 
```
brew doctor
```

- See what the Doctor says.  You may need to edit your ~/.bashrc
```bash
echo 'export PATH="/usr/local/bin:/usr/local/sbin:~/bin:$PATH"' >> ~/.bash_profile
```


## Git

Sign up for an account on [http://www.github.com](http://www.github.com). We will be using github.com for storing and sharing code.


###Install git
```
brew install git
```


###Update git config information
Eventually you'll want to configure your github settings to use your account.

```
git config --global user.name "YOUR-USERNAME"
git config --global user.email YOUR-EMAIL-ADDRESS
git config --global credential.helper cache
```


##RVM and Ruby
RVM is a Ruby Version Manager. It lets you easily switch between ruby versions.

###Install RVM with Ruby

[http://www.rvm.io](http://www.rvm.io) for full instructions


Running the following command will install the latest version of Ruby as well as the RVM envionment into your session.

```
\curl -L https://get.rvm.io | bash -s stable --ruby --rails
```

![image](./install_rvm.png)


##Rails

###Install Rails 4
After you have installed ruby, we will install a version of rails 3 for the class.

```
gem install rails
```

---
---



#Ubuntu Instructions 



##apt-get

###Install apt-get
```
sudo apt-get install curl
```

##rvm & ruby

###Install RVM
```
\curl -L https://get.rvm.io | bash -s stable --ruby --rails
```


###Login Shell preference
- In terminal go to `Edit -> Profile Preferences`
- Under `Title and Command` check `Run command as a login shell`
- Close preferences and restart terminal



##rails

###Install Rails 3.2.15
```
gem install rails -v "3.2.15"
```


##git

###Install git
```
sudo apt-get install git-core
```

###Update git config information

```
git config --global user.name "YOUR-USERNAME"
git config --global user.email YOUR-EMAIL-ADDRESS
git config --global credential.helper cache
```

---
---
#Windows Users

We recommend that you install a Linux distribution like Ubuntu on your computer and boot into Linux.
