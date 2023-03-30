# asdf-scala-cli

Plugin to manage [Scala CLI](https://github.com/VirtusLab/scala-cli), a command-line tool to interact with the Scala language. It lets you compile, run, test, and package your Scala code (and more!)

:rotating_light: **NOTE:** Commits to this repository are [automatically mirrored](https://docs.gitlab.com/ee/user/project/repository/mirror/) to a **PUBLIC** repository. This is to allow `asdf` to access and add the plugin. :rotating_light:

For details on `asdf` plugin development, see the `asdf` documentation on how to [create a plugin](https://asdf-vm.com/plugins/create.html).

## How to install

### Build dependencies

To download and build `scala-cli`, the plugin only depends on `curl`. The dependencies are taken care of by the `scala-cli` standalone script.

### Adding the plugin

To make the plugin available for `asdf`, it is published through a [public mirror repository](https://github.com/Colin-TUE/asdf-scala-cli). Add `asdf-scala-cli` by pointing to the mirror:

```shell
asdf plugin add scala-cli https://github.com/Colin-TUE/asdf-scala-cli
```

### Updating the plugin

To update the plugin, run the following command:

```shell
asdf plugin update scala-cli
```

Then it might be needed to reinstall the plugin.
This assume that the plugin is part of your `.tool-versions`.

```shell
asdf uninstall scala-cli
asdf install
```

### Installing the tool

Now install the `skopeo` tool provided by the plugin:

```shell
asdf install scala-cli latest
```
