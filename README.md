StjornvisiWeb
=============

The Whole Stjórnvísi Web Application

After cloning, remember to run

    $ php composer.phar install

It would be a good idea to create a directory some were on yoy hard drive, call it *images*, then create subdirectories
called *60*, *100*, *300*, *original* and softlink it to /public/stjornvisi/images. Just make sure that everybody has
read and write permissions to it.

It would also be a great idea to set /data/search read- and writable for everyone.

Now you need all JS/CSS dependencies. navigate to /public/stjornvisi and run

    $ bower install


