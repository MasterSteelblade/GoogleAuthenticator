# Google Authenticator

This package provides Google Authenticator functionality to your sites. 

Documentation is pending. 

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
Please use GitHub issues for support, as they're the easiest way to get in touch with me. Feel free to submit feature requests and bug reports, and I'll do what I can to implement them! 

If you think you found a bug or you have a feature idea to propose, feel free to open an issue
**after looking** at the [contributing guide](CONTRIBUTING.md).

## License

This package is available under the [MIT license](LICENSE), and was originally forked from the seemingly abandoned [Sonata Project](https://github.com/sonata-project/GoogleAuthenticator) fork.
