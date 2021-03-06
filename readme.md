# Laravel Homestead FORK

Major changes are:
 * [Mailcatcher](http://mailcatcher.me) to catch and view mails sent by server
 * ZSH shell with [grml-zsh-config](http://grml.org/zsh/)
 * PhpMyAdmin on port 1085 / 10850
 * Minor tweaks and aliases for artisan and behat

For more info or feature requests look here: https://github.com/cgrossde/settler

Official documentation [is located here](http://laravel.com/docs/homestead?version=4.2).


## Use

This box is available as `cgrossde/homesteadfork`. Fetch it using vagrant:

```
vagrant box add cgrossde/homesteadfork
```

To use this box you need my fork of [homestead](https://github.com/cgrossde/homestead). Install it using `composer` like this:

```
composer global require "cgross/homesteadfork"
```

After that you will have the `hsfork` command. The rest of the install is equivalent with the [Laravel documentation](http://laravel.com/docs/4.2/homestead) about homestead. Just replace every `homestead` command with the `hsfork` command. I renamed it to `hsfork` so you can install homestead and my fork in parallel but you won't be able to run both machines at the same time since they use the same ports.
