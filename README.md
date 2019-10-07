# MessageCloud Coding Standard

The PHP coding standard for MessageCloud.

## Installation

1. Require the package in your `composer.json`:
```json
{
  "require-dev": {
    "messagecloud/messagecloud-coding-standard": "^3.0"
  }
}
```

2. Create a PHP Code Sniffer configuration file `phpcs.xml`:
```xml
<?xml version="1.0"?>
<ruleset name="MessageCloud Coding Standard">
    <rule ref="./vendor/messagecloud/messagecloud-coding-standard/ruleset.xml"/>

    <!-- Path to check -->
    <file>./src</file>
</ruleset>
```