[![Github All Releases](https://img.shields.io/github/downloads/DBezemer/rpm-haproxy/total.svg)](https://github.com/DBezemer/rpm-haproxy/releases)

# A Recipe for a HAProxy 1.9 stable version RPM on CentOS / RHEL / Amazon Linux

Perform the following on a build box as a regular user.

## Install Prerequisites for RPM Creation

    sudo yum groupinstall 'Development Tools'

## Checkout this repository

    cd /opt
    git clone https://github.com/DBezemer/rpm-haproxy.git 
    cd ./rpm-haproxy
    git checkout 1.8

## Build using makefile
    make
    
Resulting RPM will be in /opt/rpm-haproxy/rpmbuild/RPMS/

## Credits

Based on the Red Hat 6.4 RPM spec for haproxy 1.4 combined with work done by 
- [@nmilford](https://www.github.com/nmilford)
- [@resmo](https://www.github.com/resmo) 
- [@kevholmes](https://www.github.com/kevholmes)
- Update to 1.8 contributed by [@khdevel](https://github.com/khdevel)
- Amazon Linux support contributed by [@thedoc31](https://github.com/thedoc31)

Additional logging added based on https://www.percona.com/blog/2014/10/03/haproxy-give-me-some-logs-on-centos-6-5/
