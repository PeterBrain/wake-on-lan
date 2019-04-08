# Wake on LAN
Wake-On-LAN (WOL) starts your computer remotely... magic

First of all, this is the structure of the needed database named 'server'.
```sql
CREATE TABLE `server`.`wol` (
 `owner_id` INT(11) NOT NULL COMMENT 'User ID',
 `name` VARCHAR(50) NOT NULL COMMENT 'Name',
 `ip` VARCHAR(50) NOT NULL COMMENT 'IP-Adress',
 `mac` VARCHAR(50) NOT NULL COMMENT 'MAC-Adress',
 `shared` TINYINT(1) NOT NULL COMMENT 'visible to everyone',
 UNIQUE `name` (`name`)
) ENGINE = InnoDB;
```

Put this into your PHP script to send a Magic Packet
```php
require_once __DIR__.'\wakeonlan.php';
\wakeol\WakeOnLAN::wakeUp($mac, $ip);
```
