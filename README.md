# 2020.rustfest.eu

This repo contains the website of RustFest Global 2020

## local build

### inside a docker container

To build the blog locally with docker run the following command:
```
docker run --rm --volume=$(pwd):/srv/jekyll -p 35729:35729 -p 4000:4000 -it jekyll/jekyll jekyll serve
```

Do not forget to clear the image every now and then:
```
docker rmi jekyll/jekyll
```

### native ruby installation

If your machine is already setup with ruby use this command for the latest version of all packages:
```
rm Gemfile.lock && bundle install && jekyll serve
```
