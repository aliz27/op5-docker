FROM centos:centos6
RUN yum install -y iptables
RUN curl -L -o /tmp/op5.tar.gz http://www.op5.com/?wpfb_dl=647 \
	&& cd /tmp && tar zxvf op5.tar.gz \
	&& cd /tmp/op5-monitor-* \
	&& ./install.sh --silent --offline \
	&& rm -rf /tmp/op5*
