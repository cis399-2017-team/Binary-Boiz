
Administration Doc
------------------
 1. We created a pupped module to make sure that all the package prerequisites are installed for paperwork
 2. We followed the [instructions](https://github.com/twostairs/paperwork/wiki/Installing-Paperwork-on-Ubuntu-16.04-lts) in the paperwork documentation for the initial setup of a LEMP server to run the application
 3. We had some trouble with running **composer install** command, so after some researching it turns out we need more ram so we temporarly upgraded our instance from nano to micro. Also we got two other errors that are:
    * Cannot create cache directory /home/webadmin/.composer/cache/repo/https---packagist.org/, or directory is not writable. Proceeding without cache. Cannot create cache directory /home/webadmin/.composer/cache/files/, or directory is not writable. > Cannot create cache directory /home/webadmin/.composer/cache/files/, or directory is not writable. Proceeding without cache.
       * this was solved by running this command: **sudo chown -R $USER $HOME/.composer**/
    * [RuntimeException] vendor does not exist and could not be created
       * * this was solved by running this command: **chmod -R 777 /var/www**.
 3. Then we created an SSL certificate to add encryption to our data.  We followed instructions on [this](https://www.digitalocean.com/community/tutorials/how-to-create-an-ssl-certificate-on-nginx-for-ubuntu-14-04) website.
