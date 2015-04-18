```yaml
name:                 # string
version:              # string
description:          # string
keywords:             # array
homepage:             # string
bugs:                 # object
  url:                # string
  email:              # string
license:              # string
author:               # object
  name:               # string
  email:              # string
  url:                # string
contributors:         # array of objects
  - name:             # string
    email:            # string
    url:              # string
files:                # array of strings
main:                 # string
bin:                  # object
  $name:              # string
man:                  # string || array of strings
repository:           # object
  type:               # string
  url:                # string
scripts:              # object
dependencies:         # array of objects
  $name:              # string
devDependencies:      # array of objects
  $name:              # string
peerDependencies:     # array of objects
  $name:              # string
bundleDependencies:   # array of objects
  $name:              # string
optionalDependencies: # array of objects
  $name:              # string
engines:              # array of objects
  $name:              # string
os:                   # array of strings
cpu:                  # array of strings
private:              # boolean
```