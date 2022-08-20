FROM ubuntu 
RUN apt update 
RUN apt install –y apache2 apache2-utils 
RUN apt autoremove -y
RUN apt clean 
COPY ./html /var/www/html
EXPOSE 80
CMD [“apache2ctl”, “-D”, “FOREGROUND”]