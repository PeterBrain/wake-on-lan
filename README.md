[![GitHub followers](https://img.shields.io/github/followers/peterbrain.svg?style=social&label=Follow)](https://github.com/peterbrain)
[![GitHub watchers](https://img.shields.io/github/watchers/peterbrain/wake-on-lan.svg?style=social&label=Watch)](https://github.com/peterbrain/scripts)
[![GitHub stars](https://img.shields.io/github/stars/peterbrain/wake-on-lan.svg?style=social&label=Star)]()
[![GitHub forks](https://img.shields.io/github/forks/peterbrain/wake-on-lan.svg?style=social&label=Fork)]()

[![GitHub author](https://img.shields.io/badge/Author-PeterBrain-3BCDD6.svg)](http://peterbrain.github.io)
[![GitHub author](https://img.shields.io/badge/language-PHP-8892BF.svg)]()

# Wake on LAN
Wake-On-LAN (WOL) starts your computer remotely... magic

 First of all, this is the structure of the needed database named 'server'.
````
CREATE TABLE `server`.`wol` (
 `owner_id` INT(11) NOT NULL COMMENT 'User ID',
 `name` VARCHAR(50) NOT NULL COMMENT 'Name',
 `ip` VARCHAR(50) NOT NULL COMMENT 'IP-Adress',
 `mac` VARCHAR(50) NOT NULL COMMENT 'MAC-Adress',
 `shared` TINYINT(1) NOT NULL COMMENT 'visible to everyone',
 UNIQUE `name` (`name`)
) ENGINE = InnoDB;
````

More soon
