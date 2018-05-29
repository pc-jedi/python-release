# python

To vendor python package into your release, run:

```
$ bosh vendor-package python-<version> ~/workspace/bosh-packages/python-release
```

Included packages:

- python-2.7
- python-3.6

To use `python-*` package for compilation in your packaging script:

```bash
#!/bin/bash -eu
source /var/vcap/packages/python-<version>/bosh/compile.env
pip install ...
```
