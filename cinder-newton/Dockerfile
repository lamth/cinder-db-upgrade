FROM centos:7

COPY ./etc/yum.repos.d/openstack-newton.repo /etc/yum.repos.d/openstack-newton.repo 

RUN yum install -y python-pip python-openstackclient mariadb python2-PyMySQL openstack-cinder

RUN pip install keystonemiddleware==4.6.0

COPY ./etc/cinder/cinder.conf /etc/cinder/cinder.conf

RUN mkdir /root/results

CMD tail -f /dev/null



