# docker-ceph-container

[![Build Status](https://travis-ci.org/osism/docker-ceph-container.svg?branch=master)](https://travis-ci.org/osism/docker-ceph-container)
[![Docker Hub](https://img.shields.io/badge/Docker%20Hub-osism%2Fceph-daemon-blue.svg)](https://hub.docker.com/r/osism/ceph-daemon/)

Ubuntu images have not been provided by the ``ceph-container`` upstream since the
end of August 2018.

This image is a workaround to seamlessly migrate environments running on
Ubuntu images to CentOS images.

Due to this workaround, it is not necessary to adjust the existing file
permissions of ``/var/lib/ceph`` during the rolling update.

To use this container it is necessary to always set the ``ceph_uid`` fact in
``ceph-ansible`` to ``64045``.

License
-------

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Author information
------------------

This Docker image was created by [Betacloud Solutions GmbH](https://www.betacloud-solutions.de).

Notices
-------

Docker and the Docker logo are trademarks or registered trademarks of Docker, Inc. in the
United States and/or other countries. Docker, Inc. and other parties may also have trademark
rights in other terms used herein.
