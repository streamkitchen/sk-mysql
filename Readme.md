sk-mysql
--------

The regular mysql image doesn't work well in Kubernetes, because there's a `lost-and-found`
directory present in the place it wants to make this directory. This image patches the `my.cnd`
file to ignore that directory.
