# multi-arch-circleci-and-insecure-docker-registry

It took me some time to get the configuration to work, so I share it. Maybe it can be usefull to others too.

What it does is quite simple: I have a python file, and I want to build a docker image from it. This image is in fact a bundle of 3 images:
- One for intel platform (amd64 architecture).
- One for arm platform (arm/v7 architecture).
- One for arm platform PI 4 model B (arm64 architecture).
Then it pushes the image to a remote private insecure registry.
