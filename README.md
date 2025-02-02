[![Marketplace](https://img.shields.io/vscode-marketplace/v/IBM.codewind.svg?label=marketplace&logo=visual-studio-code)](https://marketplace.visualstudio.com/items?itemName=IBM.codewind)
[![License](https://img.shields.io/badge/License-EPL%202.0-red.svg?label=license&logo=eclipse)](https://www.eclipse.org/legal/epl-2.0/)
[![Build Status](https://ci.eclipse.org/codewind/buildStatus/icon?job=Codewind%2Fcodewind-vscode%2Fmaster)](https://ci.eclipse.org/codewind/job/Codewind/job/codewind-vscode/job/master/)
[![Chat](https://img.shields.io/static/v1.svg?label=chat&message=mattermost&color=145dbf)](https://mattermost.eclipse.org/eclipse/channels/eclipse-codewind)

# Codewind for VS Code
Create and develop cloud-native, containerized web applications from VS Code.

## Installing Codewind
You can install Codewind locally in VS Code. For more information about installing Codewind, see [Installing Codewind for VS Code](https://www.eclipse.org/codewind/mdtvscinstallinfo.html).

Prerequisites
- Install [VS Code](https://code.visualstudio.com/download).
- Install Docker.
- If you use Linux, you also need to install Docker Compose.

Complete the installation:
1. Find Codewind for VS Code in the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.codewind) or by searching for `Codewind` in the [VS Code Extensions view](https://code.visualstudio.com/docs/editor/extension-gallery#_browse-for-extensions).
2. Open the **Codewind** view in the Explorer view group or enter `Focus on Codewind View` into the [**Command Palette**](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette). If you do not see the Codewind view in either the Explorer view or the **Command Palette**, the extension did not install correctly.
3. Codewind requires the installation of additional Docker images to run. Choose **Install** when prompted to complete the installation. The installation may take a few minutes to complete. Codewind creates a folder called `codewind-workspace` within your home directory to contain your projects. On Windows, this is the `C:\codewind-workspace` directory. When the installation is complete, you can open the `codewind-workspace` folder or a project within the workspace as your VS Code workspace. The tools offer to open the workspace for you if it’s not open already.

## Using Codewind for VS Code
To see the actions available, open the [**Command Palette**](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette) and type `Codewind`.</br>

Features:</br>
- [**Create New Project** and **Add Existing Project**](mdt-vsc-commands-project.html): Create new projects from application templates or import existing container-ready projects.
- [**Codewind view**](mdt-vsc-commands-project.html): View Codewind projects, including application and build statuses.
- [**Attach debugger**](mdt-vsc-commands-restart-and-debug.html): Debug Microprofile, Spring, and Node.js projects in their containers.
- [**Show all logs**](mdt-vsc-commands-project.html): View application and build logs in the VS Code **Output** view.
- [**Open folder as workspace**](mdt-vsc-commands-project.html): View and edit project deployment information.
- [**Open container shell**](mdt-vsc-commands-project.html): Open a shell session into a Codewind application container.
- [**Toggle auto build**](mdt-vsc-commands-project.html): Toggle project auto build and manually initiate project builds.
- [**Enable or disable project** and **Show project overview**](mdt-vsc-commands-project.html): Disable, enable, and delete projects.

## Contributing
Submit issues and contributions:
- [Submitting issues](https://github.com/eclipse/codewind/issues)
- [Contributing](CONTRIBUTING.md)
- [Development Builds](https://download.eclipse.org/codewind/codewind-vscode/)
- [Jenkins](https://ci.eclipse.org/codewind/job/Codewind/job/codewind-vscode/)
- To host the extension yourself so you can develop or debug it, clone this repository and run the **Extension** launch in `dev/.vscode/launch.json`. See [Developing Extensions](https://code.visualstudio.com/docs/extensions/developing-extensions) for more information.
- You can also build the extension `.vsix` yourself by running [`vsce package`](https://code.visualstudio.com/api/working-with-extensions/publishing-extension#packaging-extensions) from `dev/`. Refer to the [`Jenkinsfile`](https://github.com/eclipse/codewind-vscode/blob/master/Jenkinsfile) to see the exact steps the build runs.
