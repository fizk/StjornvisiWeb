StjornvisiWeb
=============







	$ cd ~/workspace
	$ git clone https://github.com/fizk/StjornvisiWeb.git SV
	$ git submodule init
	$ git submodule -q foreach git pull -q origin master

    $ php composer.phar install

	$ ln -s ~/workspace/SV/module/Stjornvisi/public/stjornvisi ~/workspace/SV/public/stjornvisi
	$ ln -s ~/workspace/_stjornvisi-images ~/workspace/SV/module/Stjornvisi/public/images

	$ cp ~/workspace/SV/config/autoload/stjornvisi.local.php.dist ~/workspace/SV/config/autoload/stjornvisi.local.php


    $ cd module/Stjornvisi/public/stjornvisi
    $ bower install


The Whole Stjórnvísi Web Application

After cloning, remember to run

    $ php composer.phar install

It would be a good idea to create a directory some were on yoy hard drive, call it *images*, then create subdirectories
called *60*, *100*, *300*, *original* and softlink it to /public/stjornvisi/images. Just make sure that everybody has
read and write permissions to it.

It would also be a great idea to set /data/search read- and writable for everyone.

Now you need all JS/CSS dependencies. navigate to /public/stjornvisi and run

    $ bower install


