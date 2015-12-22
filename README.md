# jekyll-development-environment
Docker scripts that let you run Jekyll without installing ruby. Supports windows and linux


[Docker for Windows](https://www.docker.com/docker-toolbox)
[Docker for Linux](https://docs.docker.com/engine/installation/)
[Docker Machine for Linux](https://docs.docker.com/machine/install-machine/)

Add the appropriate scripts to the root directory of your project, rename them if you prefer eg:
Linux:
linux-start -> start
linux-publish -> publish

Windows:
windows-start -> start
windows-publish -> publish


Now you can develop your project in docker by just running(this will build the site, and serve it on a URL that will be displayed to you.  This build will include draft posts) 
`$ ./start`

When your done developing run  (This does the same as above, but will NOT include draft posts):
`$ ./publish`


Once your happy with your site, upload the dist folder to your favorite hosting provider.