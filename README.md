Sentry on Heroku
================

    Sentry_ is a realtime event logging and aggregation platform.  At its core
    it specializes in monitoring errors and extracting all the information
    needed to do a proper post-mortem without any of the hassle of the
    standard user feedback loop.

    .. _Sentry: https://github.com/getsentry/sentry


Basic setup
-----------

Follow the steps below to get Sentry up and running on Heroku:

1. [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

2. Run Sentry's database migrations::

        heroku run "sentry --config=sentry.conf.py upgrade"

3. Create a user account for yourself::

        heroku run "sentry --config=sentry.conf.py createsuperuser"

That's it!
