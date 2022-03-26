FROM nginx:1.20.2

COPY ./conf/nginx.conf /etc/nginx/nginx.conf

# install debug tools
RUN apt-get update && apt-get upgrade -y
RUN apt-get install --no-install-recommends -y \
    make \
    neovim \
    lsof \
    apache2-utils

CMD ["nginx", "-g", "daemon off;"]

