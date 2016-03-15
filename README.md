Homewbrew is a package manager, it's like installing an app on your phone except cooler because you feel like you're hacking the matrix. A developer will use many different ones (gem, npm, bower, etc) right now we're installing HomeBrew which will install your core Mac packages.

This file will install all homebrew packages needed for class

First copy and paste this into your terminal to install the homebrew package manage:

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)`

We're going to install one package that will run a script and automate the rest of the packages we need

The package we need is **Homebrew-bundle** (it will bundle our packages together and install them all)

Copy and paste this into your terminal:

`brew tap Homebrew/bundle`

Now that we have the bundler installed go to your root directory by typing: `cd ~`

Then run copy and paste this **entire block at once** and hit enter: 

```
echo "tap 'homebrew/bundle'
tap 'homebrew/dupes'
tap 'homebrew/versions'
brew 'node'
brew 'tmux'
brew 'vim'
brew 'wemux'
brew 'git'" > Brewfile
```

This automatically creates a file with all the packages we're going to install in the bundle.

Now we're going to use our bundler by running 

`brew bundle`

That's it :100: don't worry about how all this works too much, it's grunt work that just has to be done to set everything up. 


