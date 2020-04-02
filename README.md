Flask-Session
=============

Flask-Session is an extension for Flask that adds support for Server-side Session to your application.


What's New
----------

The original package was at its version 0.3.1,
and its latest github commit activity happened 3 years ago.

Its file-based session feature stops working since its underlying package,
werkzeug, released 1.0.0 at Feb 6, 2020.
See [bug report here](https://github.com/fengsp/flask-session/issues/112).

This fork serves as a workaround to fix that issue.


How to Install
--------------

I do not have ownership of the original package "flask-session" on PyPI,
so I can not publish this there,
therefore normal "pip install package_name" would NOT work.

To use this package, you have to get it from github directly.

    pip uninstall flask-session  # Do this if you already installed the old flask-session 0.3.1
    pip install git+https://github.com/rayluo/flask-session.git@0.3.x

Or you can put this into your `requirements.txt` or `setup.py`:

    package-foo==1.2.3
    git+https://github.com/rayluo/flask-session@0.3.x#egg=flask-session
    package-bar>=2,<3

Known issue
-----------

Do this if you already installed the old flask-session 0.3.1,
because the unusual installation method mentioned above would not upgrade it to 0.3.2.

    pip uninstall flask-session
