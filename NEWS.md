
<!-- NEWS.md is generated from NEWS.Rmd. Please edit that file -->
SnakeCharmR 1.0.3
=================

Taking measures to ensure SnakeCharmR will work properly on systems where the native encoding is not UTF-8:

-   Using Python API to check if variable is str/bytes or unicode and handling things correctly. In particular, when we read Python unicode values we flag the resulting R string as UTF-8 since that’s what we Python C API we are using will return;

-   Ensuring that Python code being executed is converted to UTF-8 and that the Python interpreter is made aware of that according to PEP 263.

SnakeCharmR 1.0.2
=================

Fixed linking and building errors on some platforms (such as Amazon Linux) by updating the autoconf file to use the correct C++ compiler preferred by R.

SnakeCharmR 1.0.1
=================

Fixed handling of NULL values in arguments, including a workaround for jeroenooms/jsonlite\#130 which was causing inconsistencies.

SnakeCharmR 1.0.0
=================

Initial release.
