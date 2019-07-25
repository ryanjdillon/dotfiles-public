# BIN

I like separating executables in bin by language, so that it is more obvious what they
are when they are lacking extensions.

With this configuration, the sub-paths in `~/bin` (e.g. `~/bin/python`) must each be
added to your `.bashrc`, `.zshrc`, `.profile`, etc.

# CRON

Just some basic pointers...

**Check if cronjobs are executed**
```
grep cron /var/log/syslog
```

**Force anacron to run cron.hourly**
```
run-parts --report /etc/cron.hourly
```
