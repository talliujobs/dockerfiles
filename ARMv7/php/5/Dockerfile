# by: Wei Lin
# date: 2015/9/14

FROM wei1234c/ubuntu_armv7

MAINTAINER Wei Lin

ENV TERM linux 


# Install php _______________________________________________________________________________________________
RUN \
     apt-get update && \
     apt-get install -y php5 php5-cgi php5-cli php5-common php5-curl php5-dbg php5-dev php5-exactimage php5-fpm \
     php5-gd php5-gmp php5-imap php5-intl php5-json php5-ldap php5-memcache php5-memcached php5-mongo php5-mysql \
     php5-oauth php5-odbc php5-pgsql php5-pspell php5-readline php5-recode php5-redis php5-sqlite php5-sybase php5-tidy \
     php5-xdebug php5-xmlrpc php5-xsl

RUN  \
     apt-get install -y php5-mysqlnd  php5-mysqlnd-ms
    
# Define default command.
CMD ["bash"]



# Misc. ______________________________________________________________________________________________________

# Upgrade and clean up
RUN \
     apt-get dist-upgrade -y && \
     apt-get autoremove -y && \
     apt-get autoclean -y && \
     apt-get clean -y && \
     rm -rf /var/lib/apt/lists/*