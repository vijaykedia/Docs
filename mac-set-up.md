# Steps to set up fresh mac
- [Customize Settings](#customize-settings)
- [Basic Apps](#basic-apps)
- [Developer Tools](#developer-tool) 


## Customize Settings

- Go to Settings -> Trackpad -> toggele `Tap to click` to on.
- Go to Settings -> Desktop & Dock -> toggle `Minimise windows into application icon` to on.
- Go to Settings -> Desktop & Dock -> toggle `Show suggested and recent apps in Dock` to off.

## Basic Apps

- **Install Rectange** - Rectangle is a window management app for macOS that serves as an actively maintained alternative to Spectacle. It’s a handy utility for organizing and resizing windows efficiently. You can download it from [here](https://rectangleapp.com).

- **Install xcode** - Many command-line tools on macOS require acceptance of Xcode's terms and conditions. To ensure compatibility, install Xcode and the necessary developer tools from the App Store, then launch Xcode to accept the license agreement.

- **Install 1password** - 1Password is a password management app that helps you securely store and access your credentials. You can install it from [here](https://1password.com/downloads/mac) and log in to your account to get started.

- **Install Chrome** - Chrome is a popular alternative to Safari for browsing the web on macOS. You can install it from [here](https://www.google.com/intl/en_in/chrome/) and sign in to sync your history, bookmarks, extensions, and other settings across devices.

- **Install Visual Studio Code** - Visual Studio Code (VSCode) is a widely used text editor known for its flexibility and powerful features. You can install it from [here](https://code.visualstudio.com/) to start coding with ease.

- **Install iTerm2** - iTerm2 is one of the best alternatives to the default macOS Terminal, offering enhanced features and customization. You can download it from [here](https://iterm2.com/downloads.html).

- **Install Tower** - Tower is a Git GUI utility that simplifies version control with a user-friendly interface. You can install it from [here](https://www.git-tower.com/mac) and register your account to begin managing repositories efficiently.

- **Install WhatsApp** - WhatsApp is a social communication platform that allows you to send messages, make voice and video calls, and share media. You can download it from [here](https://www.whatsapp.com/download).

- **Install Jetbrains ToolBox** - JetBrains Toolbox is a utility app that helps manage the installation and updates of various JetBrains products. Download it from [here](https://www.jetbrains.com/toolbox-app/) and install it on your device. Log in using credentials associated with an active subscription to access the full suite of tools. Once toolbox is installed, install below tools from it.
  - Intellij IDEA Ultimate
  - PyCharm

- **Install Microsoft Office** - Microsoft Office is a comprehensive productivity suite that includes tools like Word, Excel, PowerPoint, and Outlook. To get started, log in [here](https://account.microsoft.com/services/microsoft365/details?openInstall=true#) and install the suite on your device.

- **Install Bitdefender** - Bitdefender is a security application designed to protect your system from malware, viruses, and other threats. To get started, log in [here](https://central.bitdefender.com) and install the protection suite on your device.

- **Install Dropbox** - Dropbox is a cloud storage application that helps you manage and sync files across devices. You can download and install it from [here](https://www.dropbox.com/install).

- **Install Microsoft Copilot** - Microsoft Copilot is a generative AI application designed to enhance productivity by integrating intelligent assistance into Microsoft 365 apps and services. Download it from [here](https://www.microsoft.com/en-us/microsoft-365/copilot/download-copilot-app).

- **Install Google Drive** - Google Drive is a cloud storage application that helps you manage and sync files across devices. You can download and install it from [here](https://dl.google.com/drive-file-stream/GoogleDrive.dmg).

## Developer Tool

- **Configure iTerm2** - If you prefer to change the default theme, you can install [`this`](./Snazzy.itermcolors) by following below instructions.
  - Launch iTerm 2.
  - Click on iTerm2 menu title
  - Select Settings... option
  - Select Profiles
  - Navigate to Colors tab
  - Click on Color Presets
  - Click on Import
  - Select the `.itermcolors` file downloaded

- **Install Zsh Batteries**: macOS uses Zsh as its default shell. To enhance its functionality, it's recommended to install additional tools and plugins using the community-driven framework [oh-my-zsh](https://ohmyz.sh/).
  ```sh
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  ```

- **Install Homebrew** - Use below command to install homebrew. Latest Instructions can be found [here](https://brew.sh/).
  ```sh
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

- **Install git**: Git is a command-line utility used for managing version control, enabling developers to track changes, collaborate, and maintain code history efficiently.
  ```sh
  brew install git
  ```

- **Install vfox**: vfox is cross platform version package manager. For installing it using Homebrew, use below command.
  ```sh
  brew install vfox
  ```

- **Install JDK**: Once vfox is installed, it can be used to install and manage multiple version of java using plugin [`vfox-java`](https://github.com/version-fox/vfox-java). Behind the scenes, `vfox-java` uses foojay api, which gives it the ability to manage java version like sdkman. For Example: To install latest version of `temurin java 21`, use below commands.
  ```sh
  # Adds java plugin to vfox
  vfox add java
  # Search and select desired version of java from the list and press enter
  vfox search java tem
  ```

- **Install Kotlin**: Once vfox is installed, it can be used to install and manage multiple version of kotlin using plugin [`vfox-kotlin`](https://github.com/version-fox/vfox-kotlin). 
  ```sh
  # Adds kotlin plugin to vfox
  vfox add kotlin
  # Search and select desired version of kotlin from the list and press enter
  vfox search kotlin
  ```

- **Install Golang**: Once vfox is installed, it can be used to install and manage multiple version of golang using plugin [`vfox-golang`](https://github.com/version-fox/vfox-golang).
  ```sh
  # Adds golang plugin to vfox
  vfox add golang
  # Search and select desired version of golang from the list and press enter
  vfox search golang
  ```

- **Install NodeJS**: Once vfox is installed, it can be used to install and manage multiple version of nodejs using plugin [`vfox-nodejs`](https://github.com/version-fox/vfox-nodejs).
  ```sh
  # Adds nodejs plugin to vfox
  vfox add nodejs
  # Search and select desired version of nodejs from the list and press enter
  vfox search nodejs
  ```

- **Install uv**: [`uv`](https://docs.astral.sh/uv/) is the python package and project manager. we can install it using homebrew.
  ```sh
  brew install uv
  ```

- **Install Python**: Since we prefer to use `uv` as python package manager, we want to install python using uv itself. Below command will install the latest stable version of python.
  ```sh
  uv python install
  ```

- **Install AWSCli** - The official AWS CLI installer from Amazon does not currently offer a universal binary for macOS, requiring Rosetta 2 for installation on Apple Silicon devices. Since Apple is rumored to phase out Rosetta support in the future, it's recommended to install AWS CLI via Homebrew for better compatibility. However, if Amazon releases a universal binary, prefer that and follow the official installation instructions available [here](https://docs.aws.amazon.com/cli/).
  ```sh
  brew install awscli
  ```
