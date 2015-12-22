# jekyll-development-environment
Docker scripts that let you run Jekyll without installing ruby. 
Supports Windows and Linux


[Docker for Windows](https://www.docker.com/docker-toolbox)

[Docker for Linux](https://docs.docker.com/engine/installation/)

[Docker Machine for Linux](https://docs.docker.com/machine/install-machine/)

Linux users will also need to install: 
[VirtualBox](https://www.virtualbox.org/wiki/Downloads)

#### To Use:
Add the appropriate scripts to the root directory of your project, rename them if you prefer (remove the OS prefix)eg:

#####Ubuntu:
    $ mv setup-docker-host /YOUR_PROJECT/setup-docker-host
	$ mv linux-start /YOUR_PROJECT/start
	$ mv linux-publish /YOUR_PROJECT/publish

##### Windows:
	$ mv setup-docker-host /YOUR_PROJECT/setup-docker-host
	$ mv windows-start /YOUR_PROJECT/start
	$ mv windows-publish /YOUR_PROJECT/publish


Now you can develop your project in docker by just running(this will build the site, and serve it on a URL that will be displayed to you.  This build will include draft posts) 

`$ ./start`


When your done developing run  (This does the same as above, but will NOT include draft posts):

`$ ./publish`

Most edits should occur without a need for restarting, if an edit does not appear, simply re-run the scripts, they are all idempotent.

Once your happy with your site, simply upload the dist folder to your favorite hosting provider.