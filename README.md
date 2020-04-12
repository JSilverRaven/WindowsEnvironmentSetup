# WindowsEnvironmentSetup
Environment setup guide for my windows machine

### Command Line Tool - cmder
- Go to https://cmder.net/
- Download latest full version (with git preinstalled)
- Unzip and move the cmder/ folder under desired path
- Edit windows environment variable, add /path/to/cmder and /path/to/cmder/bin to PATH
- Edit settings of cmder after starting one, change default startup task to `{bash::bash}`

### Package Manager - chocolatey
- Go to https://chocolatey.org/install
- Install choco through windows poershell as admin according to the instruction included above
    ```
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
    ```
- Open cmder, type `choco -v` to verify chocolatey is installed

### NodeJS and NVM
- Open cmder as admin
- Install node by running `choco install nodejs`
- Install nvm by running `choco install nvm`


### Yarn
- Get Yarn by using npm: `npm install -g yarn`
- Yarn error: `The engine "node" is incompatible with this module. Expected version "x.x.x". Got "x.x.x"`
    - Run yarn with command `--ignore-engines`


### Get Chrome Driver
- Go to https://chromedriver.chromium.org/downloads
- Download the expected chrome driver version
- Unzip and move chromdriver.exe under the `/path/to/cmder/bin/`
- Chrome driver should be now accessible

### Python
- Install using choco: `choco install python`


