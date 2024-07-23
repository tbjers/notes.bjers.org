The Bluefin team reported an issue with the signing key for the Bluefin system image affecting all installations prior to 2024-07-02.

The recommended way to fix this is described in this [forum post](https://universal-blue.discourse.group/t/important-announcement-regarding-system-updates-action-needed/2689/1).

```shell
curl -sL https://fix.universal-blue.org/ | sudo bash
```

One small caveat: the command needs to be run in the host terminal, not `bluefin-cli` or other container images.