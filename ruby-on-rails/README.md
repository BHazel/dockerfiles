# Ruby on Rails

This creates an image with the latest version of Ruby and the Ruby on Rails framework.  It is intended for development use rather than for production containers.

Recommended use is to create a container with an attached volume to the location of a Rails application source and start a shell prompt.

`docker run -it --rm -p 3000:3000 -v /path/to/rails/app:/path/in/container bash`