# vpnc-script-hooks

a collection of [vpnc-script](https://gitlab.com/openconnect/vpnc-scripts/blob/master/vpnc-script) hooks, mostly for Linux, maybe wholly for Linux,
to remediate or tune certain behaviors.  generally these operate by providing alternate sh functions.

## INSTALL

carefully examine each hook and create a symbolic link to the corresponding directory under /etc/vpnc.

### INSTALL ALL

```bash
find *.d -type f | while read f; do
  ln -s $PWD/$f /etc/vpnc/$f
done
```
