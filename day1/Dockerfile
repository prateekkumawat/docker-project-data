# base Image for update layers
FROM redhat/ubi9:latest

# Labels Setup for Image
LABEL properiters="prateek kumawat"
LABEL orgniztion="Highsky"
LABEL buid="Redhat 9"

# Install or onetime Binaries
RUN yum install nginx -y 

# use copy instruction for copy data from source to container directory
COPY src /usr/share/nginx/html/

CMD ["nginx", "-g", "daemon off;"]