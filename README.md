Apache Bigtop Custom

Version Up zookeeper 3.4.13 To 3.5.5

First, download the zookeeper source at github

git clone -b branch-3.5.5 --single-branch https://github.com/apache/zookeeper.git 

Second, Need to install Packages

# yum install openssl-devel gcc rpm-build rpm-devel rpmlint make python bash coreutils diffutils patch rpmdevtools ncyum install psmiscyum install redhat-lsb.x86_64 ant

Finally, try to rpmbuild

$ rpmbuild -ba ./SPECS/zookeeper.spec

