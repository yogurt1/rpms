# Based on Fedora 26 freetype SRPM

### How to install:
* Add these lines to /etc/yum.repos.d/yogurt1-ft27.repo:
```
[yogurt1-freetype27-x86_64]
name=Copr repo for freetype27 owned by yogurt1
baseurl=https://copr-be.cloud.fedoraproject.org/results/yogurt1/freetype27/fedora-$releasever-x86_64/
type=rpm-md
skip_if_unavailable=True
gpgcheck=1
gpgkey=https://copr-be.cloud.fedoraproject.org/results/yogurt1/freetype27/pubkey.gpg
repo_gpgcheck=0
enabled=1
enabled_metadata=1

[yogurt1-freetype27-i386]
name=Copr repo for freetype27 owned by yogurt1
baseurl=https://copr-be.cloud.fedoraproject.org/results/yogurt1/freetype27/fedora-$releasever-i386/
type=rpm-md
skip_if_unavailable=True
gpgcheck=1
gpgkey=https://copr-be.cloud.fedoraproject.org/results/yogurt1/freetype27/pubkey.gpg
repo_gpgcheck=0
enabled=1
enabled_metadata=1
```
* Update packages: ```sudo dnf upgrade``` 
