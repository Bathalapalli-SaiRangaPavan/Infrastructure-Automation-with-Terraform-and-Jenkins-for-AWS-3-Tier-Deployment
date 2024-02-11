# Visual Studio Code, Terraform, and Terragrunt Installation Guide for Windows

This guide provides step-by-step instructions for installing Visual Studio Code, Terraform, and Terragrunt on a Windows system.

## Prerequisites

- Windows operating system
- Internet connection

---

## Installing Visual Studio Code on Windows

### 1. Download the Installer

- Visit the official Visual Studio Code website at [https://code.visualstudio.com/download](https://code.visualstudio.com/download).

### 2. Download for Windows

- Click the "Download for Windows" button on the VSCode website to download the installer package appropriate for your Windows version.

### 3. Run the Installer

- Locate the downloaded installer file (usually in your Downloads folder) and double-click it to run it.

### 4. Installation Wizard

- Follow the on-screen instructions in the installation wizard:
  - Select "I accept the agreement".
  - Choose the installation location (optional).
  - Select additional tasks like adding VSCode to the system PATH or creating a desktop shortcut (optional).
  - Click "Install" to begin the installation process.

### 5. Completing the Installation

- Once the installation is complete, ensure the "Launch Visual Studio Code" option is checked, and then click "Finish".

### 6. VSCode First Launch

- Visual Studio Code will open for the first time. You're now ready to start using the editor.

---

## Installing Terraform on Windows

### 1. Download Terraform Binary

- Go to the [Terraform Downloads](https://www.terraform.io/downloads.html) page on the official Terraform website.
- Download the Terraform binary for Windows.

### 2. Extract Terraform Binary

- Once downloaded, extract the contents of the zip file to a directory of your choice on your Windows system.

### 3. Add Terraform to PATH

- Open "System (Control Panel)" > "Advanced system settings" > "Environment Variables...".
- Under "System variables", select the `Path` variable and click "Edit...".
- Add the full path to the directory where Terraform binary (`terraform.exe`) is located.
- Click "OK" on all windows to apply the changes.

### 4. Verify Installation

- Open a new command prompt window.
- Type `terraform --version` and press Enter to verify that Terraform is installed correctly.

---

## Installing Terraform Extension for Visual Studio Code

### 1. Access Extensions View

- Open Visual Studio Code.
- Click on the square icon at the bottom of the sidebar to access the Extensions view.

### 2. Search for Terraform Extension

- Type "Terraform" into the search bar and press Enter.

### 3. Install Terraform Extension

- Look for the official HashiCorp Terraform extension and click "Install".

### 4. Verify Installation

- Reload Visual Studio Code if prompted.
- After reloading, you should see the Terraform extension listed in the Extensions view under "Installed".

---

## Installing Terragrunt on Windows

### 1. Download Terragrunt

- Visit the official Terragrunt GitHub releases page: [Terragrunt Releases](https://github.com/gruntwork-io/terragrunt/releases).
- Find the latest release version and download the Windows version as a ZIP file.

### 2. Extract the Terragrunt Executable

- Extract the contents of the ZIP file to a directory of your choice.

### 3. Add Terragrunt to Your System PATH

- Right-click on the Windows Start button and select "System".
- Click on "Advanced system settings" > "Environment Variables...".
- Find and select the "Path" variable under "System Variables", then click "Edit...".
- Add the path to the directory containing the Terragrunt executable.
- Click "OK" to save the changes.

### 4. Verify the Installation

- Open a new Command Prompt and run `terragrunt --version` to verify that Terragrunt is correctly installed.

---

## Additional Resources

- [Visual Studio Code Documentation](https://code.visualstudio.com/docs)
- [Terraform Installation Documentation](https://learn.hashicorp.com/tutorials/terraform/install-cli)
- [Terragrunt Documentation](https://terragrunt.gruntwork.io/docs/)

