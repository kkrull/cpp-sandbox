#General-purpose C++ environment used to run ephemeral commands with docker run
FROM gcc:12.2
RUN apt-get update && apt-get install -y \
  cmake=3.18.4-2+deb11u1

#TODO KDK: Run interactive (or regular) and /src is empty.  Why?
#It seeems to be an issue with docker-engine only allowing volumes to be bound from certain places:
#https://stackoverflow.com/questions/34504156/docker-volume-not-mounting-any-files
WORKDIR /src
