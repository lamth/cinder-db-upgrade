FROM centos:7

COPY ./etc/yum.repos.d/openstack-newton.repo /etc/yum.repos.d/openstack-newton.repo 

RUN yum install -y python-openstackclient mariadb python2-PyMySQL openstack-cinder

COPY ./etc/cinder/cinder.conf /etc/cinder/cinder.conf

RUN mkdir /root/results

CMD tail -f /dev/null



