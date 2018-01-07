FROM mysql:5.7
MAINTAINER Romano Kleinwaechter

# enable query log
RUN \
	echo 'general_log_file = /var/log/mysql/mysql.log'    >> /etc/mysql/mysql.conf.d/mysqld.cnf && \
	echo 'general_log = 1'                                >> /etc/mysql/mysql.conf.d/mysqld.cnf && \
	echo 'long_query_time = 2'                            >> /etc/mysql/mysql.conf.d/mysqld.cnf

RUN apt-get autoremove -y && apt-get autoclean
