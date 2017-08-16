# MessageCloud Coding Standard

The PHP coding standard for MessageCloud.

## Installation

1. Require the package in your `composer.json`:
```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "git@github.com:MessageCloud/messagecloud-coding-standard.git"
    }
  ],
  "require-dev": {
    "messagecloud/messagecloud-coding-standard": "^1.0"
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
    
     <!-- Allow test methods to be snake case -->
     <rule ref="PSR1.Methods.CamelCapsMethodName">
        <exclude-pattern>./test</exclude-pattern>
     </rule>
</ruleset>
```