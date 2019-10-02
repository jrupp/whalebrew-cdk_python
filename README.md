# whalebrew-cdk_python

Whalebrew package for AWS CDK using python language

This will give you the `cdk` command from [AWS CDK](https://github.com/aws/aws-cdk), but only for python language support.  Python is preinstalled in the environment.

* Python 3.7.3
* CDK 1.10.1

Note: This container runs as root, because otherwise Node (which cdk is written in) refuses to read environment variables that are passed into the docker container.  This is because it refuses to read them unless it is running as a user that exists in passwd.

Finally: This whalebrew package requires a version of whalebrew that supports the `keep_container_user` option.  So anything greater than 0.1.0
