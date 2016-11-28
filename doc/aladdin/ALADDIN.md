# How to use django_ssl_auth with Aladdin eTokens.

## Server side:

1. set up your django app with `django_ssl_auth` as specified in the top-level README.md

1. Clone https://github.com/spron-in/django-ssl-client-auth/blob/master/django_ssl_auth/aladdin.py to your django project (smth like /path/to/project/ssl_auth)

1. To `django_ssl_auth/init.py` add `from . import aladdin`

1. In settings.py add
`USER_DATA_DN = 'ssl_auth.aladdin.parse_cert'`
