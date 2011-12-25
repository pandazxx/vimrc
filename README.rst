Quick installation
==================
Simply run this script to install and configure this vimrc in your `$HOME`
dir::

	wget -O - https://github.com/pandazxx/vimrc/raw/master/autoinstall.sh | sh

Installing this vimrc manually
==============================
Although a vimrc is a very personal thing, you may use mine if you
like it.  To do so, please do the following:

1. Clone this repo::

   	git clone git://github.com/pandazxx/vimrc.git

   or download the plain source only::

   	wget -qO - http://github.com/pandazxx/vimrc/tarball/master | tar -xzvf -

2. In your ~/.vimrc, add the following line::

   	source ~/path/to/vimrc/vimrc

3. Fetch submodules::

   	git submodule init
   	git submodule update

4. Recompile Command-T Ruby C extension for your platform (if other than
   Mac OS X)::

   	cd vim/ruby/command-t
   	ruby extconf.rb
   	make clean; make

5. Copy or link vim directory

   	ln -s ~/path/to/vimrc/vim ~/.vim

    or

   	cp -r ~/path/to/vimrc/vim ~/.vim

6. Touch::

   	touch ~/.vim/user.vim



That's it.
