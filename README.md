Opauth-Slack
=============
[Opauth][1] strategy for Slack authentication.

Implemented based on https://api.slack.com/docs/oauth

Getting started
----------------
1. Install Opauth-Slack:

   Using git:
   ```bash
   cd path_to_opauth/Strategy
   git clone https://github.com/t1mmen/opauth-slack.git slack
   ```

  Or, using [Composer](https://getcomposer.org/), just add this to your `composer.json`:

   ```bash
   {
       "require": {
           "t1mmen/opauth-slack": "*"
       }
   }
   ```
   Then run `composer install`.


2. Create Slack application at https://api.slack.com/applications

3. Configure Opauth-Slack strategy with at least `Client ID` and `Client Secret`.

4. Direct user to `http://path_to_opauth/slack` to authenticate

Strategy configuration
----------------------

Required parameters:

```php
<?php
'Slack' => array(
	'client_id' => 'YOUR CLIENT ID',
	'client_secret' => 'YOUR CLIENT SECRET'
)
```

License
---------
Opauth-Slack is MIT Licensed
Copyright © 2015 Timm Stokke (http://timm.stokke.me)

[1]: https://github.com/opauth/opauth
