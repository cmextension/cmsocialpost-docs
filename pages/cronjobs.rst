=========
Cron jobs
=========

Command line
------------

If your hosting allows you to setup and run cron job, you can create cron job to submit scheduled and queued posts of CM Social Post automatically.

You need to execute the file cmsocialpost_submit.php in "cli" folder of your Joomla! installation.

For example, with SiteGround hosting, you need to execute this command in your cron job::

    php path/to/your/joomla/cli/cmsocialpost_submit.php

With hosting which uses CloudLinux, you need to run::

    php5-cli path/to/your/joomla/cli/cmsocialpost_submit.php

You may need to contact your hosting's support staff to know what PHP command you need to run.

By default, there are only 10 posts submitted. If you want to increase this value, you can add "--limit=X" to the command, "X" is a number (there are 2 dashes in front of "limit").

For example, to submit 50 posts::

    php path/to/your/joomla/cli/cmsocialpost_submit.php --limit=50

Web based
---------

If your hosting doesn't support cron job, you can use any web based cron job services. You need to access this URL in your cron job::

    http://www.yoursite.com/index.php?option=com_cmsocialpost&task=submit&key=YOUR_KEY

"YOUR_KEY" is the key your set in CM Social Post's configuration.

Please contact your cron job service to know how to setup cron job.