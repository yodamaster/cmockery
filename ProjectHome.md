There are a variety of C unit testing frameworks available however many of
them are fairly complex and require the latest compiler technology.  Some
development requires the use of old compilers which makes it difficult to
use some unit testing frameworks.  In addition many unit testing frameworks
assume the code being tested is an application or module that is targeted to
the same platform that will ultimately execute the test.  Because of this
assumption many frameworks require the inclusion of standard C library headers
in the code module being tested which may collide with the custom or
incomplete implementation of the C library utilized by the code under test.

Cmockery only requires a test application is linked with the standard C
library which minimizes conflicts with standard C library headers.  Also,
Cmockery tries to avoid the use of some of the newer features of C compilers.

This results in Cmockery being a relatively small library that can be used
to test a variety of exotic code.  If a developer wishes to simply test an
application with the latest compiler then other unit testing frameworks may be
preferable.

For more information check out the [manual](http://cmockery.googlecode.com/svn/trunk/doc/index.html) and the [discussion group](http://groups.google.com/group/cmockery)