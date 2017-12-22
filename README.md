# Villa OS Manifest for Repo

## How to use:
```
$ repo init -u git://github.com/rose-project/villaos-manifest.git -b master
$ repo sync
```

## Build Villa OS

```
$ cd layers
$ echo "TEMPLATECONF=\${TEMPLATECONF:-meta-villa/conf}" > .templateconf
$ . oe-init-build-env 
```

You now may want to edit conf/local.conf for your needs (MACHINE variable etc.) and the run bitbake. 
```
$ bitbake villa-base-image
```
