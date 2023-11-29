# DevRev CLI

This repo provides the latest CLI release from DevRev. It is a tool that simplifies working
with the DevRev REST API.

## Debian Package

### Installation

Supported architectures:

- linux amd64
- linux arm64

Download the debian package from [here](https://github.com/devrev/cli/releases/latest)
and install it using the following command:

```bash
sudo dpkg -i devrev_0.4.0-linux_amd64.deb
```

or

```bash
sudo dpkg -i devrev_0.4.0-linux_arm64.deb
```

also run the below command to **install the completions**:

```bash
wget https://raw.githubusercontent.com/devrev/cli/main/install_completions.sh && sh install_completions.sh /usr/local/bin/devrev
```

Note: **/usr/local/bin/devrev** path may vary based on your debian installation

### Uninstallation

Use this command to deinstall the devrev debian package:

```bash
sudo dpkg -r devrev
```

---

## Homebrew

### Installation

Supported architectures:

- darwin amd64
- darwin arm64
- linux arm64
- linux amd64

Download the brew formula [devrev.rb](https://github.com/devrev/cli/releases/latest/download/devrev.rb) or run the below command:

```bash
wget https://github.com/devrev/cli/releases/latest/download/devrev.rb
```

Install the downloaded Homebrew formula file devrev.rb using below command:

```bash
brew install ./devrev.rb
```

also run the below command to **install the completions**:

```bash
wget https://raw.githubusercontent.com/devrev/cli/main/install_completions.sh && sh install_completions.sh /opt/homebrew/bin/devrev
```

Note: **/opt/homebrew/bin/devrev** path may vary based on your homebrew installation

### Uninstallation

```bash
brew uninstall devrev
```
---
## Windows

### Installation

Supported architectures:

- windows amd64

Download the windows executable from [here](https://github.com/devrev/cli/releases/latest).

Unzip the downloaded file and add the path to the environment variable.

Here are the steps on how to add a directory to your system PATH environment variable in Windows 10:

#### Steps

1. Open the System Properties window.

   There are two ways to do this:

    * Press Windows key + Pause.
    * Right-click on "This PC" in File Explorer and select "Properties."

2. In the System window, click on the "Advanced system settings" link in the left pane.

3. In the "Advanced System Properties" window, click on the "Environment Variables" button.

4. Under the "System Variables" section, select the "Path" variable and click on the "Edit" button.

5. In the "Edit environment variable" window, click on the "New" button.

6. Enter the path to the directory you want to add. For example: `C:\Program Files\devrev\`

7. Click on "OK" to save the changes.

8. Close all remaining windows by clicking on "OK".

   Note: You may need to restart your computer for the changes to take effect.


### Uninstallation

#### Steps
1. Remove the path from the environment variable.
2. Delete the downloaded executable file and its folder.

---

## Usage

The DevRev CLI provides several subcommands that can be used to perform various tasks. Here are some examples:

### CLI version

```bash
devrev --version
```

### Authentication to DevRev API

```bash
devrev profiles authenticate --org <DevOrg-slug-name> --usr <your-email@example.com>
```

**Arguments:**

`<DevOrg-slug-name>` : The unique slug name of your DevOrg to which you want to login.

`<your-email@example.com>` : Your registered user email for profile.

### CLI help

```bash
devrev --help
```

### License

DevRev CLI is proprietary software and is not open source. You may use it for your commercial use, but you may not distribute or modify it without our permission.

## Support

If you have any issues or questions about DevRev CLI, please contact our support team at [DevRev](https://devrev.ai)
