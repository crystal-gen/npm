# npm v0.1.0


[npm](http://npmjs.com) generator for [Crystal](http://crystal.sh)


# Usage

## Schema

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


## Example

```yaml
name: npm-test
version: 0.1.0

generators:
  npm:
    spec:
      private: true
      dependencies:
        - name: body-parser
          version: "~1.12.2"
        - name: cookie-parser
          version: "~1.3.4"
        - name: express
          version: "~4.12.2"
        - name: express-session
          version: "~1.10.4"
    version: latest
```


## Output

### lib/package.json

```json
{
	"name": "npm-test",
	"version": "0.1.0",
	"private": true,
	"dependencies": {
		"body-parser": "~1.12.2",
		"cookie-parser": "~1.3.4",
		"express": "~4.12.2",
		"express-session": "~1.10.4"
	}
}
```


