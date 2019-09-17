axtls for Unikraft
===================
This is the port of axtls for Unikraft as external library. You will
need lwip to make it work.

To run ssltest.c as a unit test, you'll need pthread support, e.g.,
add the following line to the LIBS variable in the Makefile:

   ...$(UK_LIBS)/lwip:$(UK_LIBS)/pthread-embedded:
      $(UK_LIBS)/newlib:$(UK_LIBS)/axtls...

Note that you'll need a filesystem in place and the certificate files for
all tests to pass.

Please refer to the `README.md` as well as the documentation in the `doc/`
subdirectory of the main unikraft repository.
