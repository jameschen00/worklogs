# worklogs

This is a worklogs plugin for Redmine.


## Installation

To install the plugin, execute the following commands from the root of your Redmine directory:

```
cd plugins
git clone https://github.com/IceskYsl/worklogs.git
```

and then execute the following commands from the root of your Redmine directory:

```
$ RAILS_ENV=production rake redmine:plugins:migrate
```	

More information on installing Redmine plugins can be found at [redmine.org](http://www.redmine.org/wiki/redmine/Plugins.).

After the plugin is installed you will need to restart Redmine for the plugin to be available.

## Task

Add the task into crontable
```
$ cat /etc/cron.daily/week.sh
#!/bin/bash
PATH=/sbin:/bin:/usr/sbin:/usr/bin:/opt/ruby/bin
cd /opt/redmine/
RAILS_ENV=production bundle exec rake worklogs:day
```

### Uninstallation

To remove the plugin, from the root of your installation directory do the following:
```
rm -rf plugins/worklogs
bundle install
```

## Demo
Configure
![Configure](https://f.cloud.github.com/assets/5537/756005/899aab90-e5d5-11e2-8b0c-a92bef0644c4.png)

![Configure](https://f.cloud.github.com/assets/5537/756006/8d375c3a-e5d5-11e2-9377-ad887a58a6db.png)

demo
![pic](https://f.cloud.github.com/assets/5537/719898/31cfb77e-dfa0-11e2-8618-6dd6c6bc31fd.jpg)

