![Sentry](http://img.dafont.com/preview.php?text=Sentry&ttf=squared_display0&ext=1&size=64&psize=m&y=53)
================

[Sentry](http://github.com/getsentry/sentry) is a realtime event logging and aggregation platform.  

At its core it specializes in monitoring errors and extracting all the information needed to do a proper post-mortem without any of the hassle of the standard user feedback loop.


Basic setup
-----------

Follow the steps below to get Sentry up and running on Heroku:

1. [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

2. Run Sentry's database migrations::

        heroku run "sentry --config=sentry.conf.py upgrade"

3. Create a user account for yourself::

        heroku run "sentry --config=sentry.conf.py createsuperuser"

That's it!
