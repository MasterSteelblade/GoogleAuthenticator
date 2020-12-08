# Google Authenticator

Ported from http://code.google.com/p/google-authenticator/

You can use the Google Authenticator app from here
http://www.google.com/support/accounts/bin/answer.py?hl=en&answer=1066447
to generate One Time Passwords/Tokens and check them with this little
PHP app (Of course, you can also create them with this).

Branch | Github Actions |
------ | -------------- |
master | [![Test](https://github.com/MasterSteelblade/GoogleAuthenticator/workflows/Test/badge.svg)](https://github.com/MasterSteelblade/GoogleAuthenticator/actions?query=workflow%3ATest+branch%3Amaster) |


## Requirements

This fork is built for PHP 8.0+.

## Installation using Composer

```bash
composer require mastersteelblade/google-authenticator
```

## Usage

See example.php for how to use it.

There's a little web app showing how it works in web/, please make users.dat
writeable for the webserver, doesn't really work otherwise (it can't save the
secret). Try to login with chregu/foobar.

What's missing in the example:

 * Prevent replay attacks. One token should only be used once
 * Show QR Code only when providing password again (or not at all)
 * Regenerate secret

## Support
Please use GitHub issues for support, as they're the easiest way to get in touch with me. 

If you think you found a bug or you have a feature idea to propose, feel free to open an issue
**after looking** at the [contributing guide](CONTRIBUTING.md).

## License

This package is available under the [MIT license](LICENSE), and was originally forked form [Sonata Project](https://github.com/sonata-project/GoogleAuthenticator).
