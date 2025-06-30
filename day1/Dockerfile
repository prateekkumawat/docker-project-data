# base Image for update layers
FROM redhat/ubi9:latest

# Labels Setup for Image
LABEL properiters="prateek kumawat"
LABEL orgniztion="Highsky"
LABEL buid="Redhat 9"

# Install or onetime Binaries
RUN yum install httpd -y 

# use copy instruction for copy data from source to container directory
COPY src /var/www/html/ 

CMD ["/usr/sbin/httpd", "-DFOREGROUND"]