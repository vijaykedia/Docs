# Steps to set up fresh mac
- **Install iTerm2** - One of the best alternative to default mac terminal. It can be downloaded from [here](https://iterm2.com/downloads.html). If you prefer to change the default theme, you can install [`this`](./Snazzy.itermcolors) by following below instructions.
  - Launch iTerm 2.
  - Click on iTerm2 menu title
  - Select Settings... option
  - Select Profiles
  - Navigate to Colors tab
  - Click on Color Presets
  - Click on Import
  - Select the `.itermcolors` file downloaded
- **Install Zsh Batteries**: Mac uses zsh as the default shell. If you want to change the default shell, you can refer the instruction from [here](https://support.apple.com/en-in/guide/terminal/trml113/mac). If you prefer to us zsh instead, it's better to install zsh batteries via a community driven framework [`oh-my-zsh`](https://ohmyz.sh/).
  ```sh
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  ```
- **Install Homebrew** - Use below command to install homebrew. Latest Instructions can be found [here](https://brew.sh/).
  ```sh
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
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
- **Install git**: - Use homebrew to install git
  ```sh
  brew install git
  ```
- Install AWSCli by download latest GUI installer from [here](https://awscli.amazonaws.com/AWSCLIV2.pkg). For reference: Always validate the instructions from [here](https://docs.aws.amazon.com/cli/).