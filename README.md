alertmanager-telegram-bot
=========

Installs and sets up
[alertmanager-bot](https://github.com/metalmatze/alertmanager-bot), a service
relaying Alertmanager alerts via Telegram.

Requirements
------------

Implicitly: A Telegram account, a Telegram bot and a running Alertmanager
instance.

Role Variables
--------------

| Variable Name | Default Value | Description |
`alertmanager_telegram_bot_admin` | "" | **required**, the admin account for the telegram bot
`alertmanager_telegram_bot_token` | "" | **required**, the token for the telegram bot
`alertmanager_telegram_bot_version` | "0.4.0" | Version of alertmanager-bot to install
`alertmanager_telegram_bot_checksum` | "sha256 |1f2f7c741267db386f7fadc5758636e22ca27bc3f22c6da4fa278ca88e2c148c" | Hash of the downloaded binary
`alertmanager_telegram_bot_alertmanager_url` | "http://127.0.0.1:9093" | URL of the Alertmanager instance
`alertmanager_telegram_bot_listen_addr` | "127.0.0.1:18000" | URL that Alertmanager sends alerts to
`alertmanager_telegram_bot_user` | "alertmanager-bot" | User to create and run as

Dependencies
------------

None.

Example Playbook
----------------

See `molecule/default/playbook.yml`.

License
-------

BSD

Author Information
------------------

Find me on [GitHub](https://github.com/ThreeFx).
