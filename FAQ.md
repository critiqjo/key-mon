# FAQ #

**Q:** I installed the debian package on my Debian machine and got the following error

```
$ key-mon

Traceback (most recent call last):
  File "<string>", line 1, in <module>
ImportError: No module named keymon.key_mon
```

**A:** You probably don't have python2.6 installed, and that is where the debian package installs to.  If you install from source (.zip or .tar.gz) you shouldn't experience this problem since it uses whichever python is the default.