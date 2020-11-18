FROM debian:sid
RUN sed -i 's#http://deb.debian.org#http://mirrors.163.com#g' /etc/apt/sources.list

RUN apt-get update && apt-get install nginx wrk curl wget s3fs skopeo podman buildah git fuse -y

CMD ["nginx", "-g", "daemon off;"]