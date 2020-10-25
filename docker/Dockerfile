FROM centos:7
RUN yum install -y epel-release && \
    yum install -y nginx 
RUN sed -i '/\:\:/s/^/#/' /etc/nginx/nginx.conf
COPY index.html /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
