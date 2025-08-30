# DemoCodespaces
This is a demo of a sample codespaces repo and how to create it.

Install the Github CodeSpaces in the VS code extentions marketplace. Then create a codespace and add a repository to it (where data will be stored). Next, click on the three lines in the codespaces and click on open in VS Code. This will redirect you to the VS code on your local machine and you can access your codespaces from the terminal.

### Install terraform on Codespaces:

Go to https://developer.hashicorp.com/terraform/install and copy the install command for Ubuntu/Debian and paste it into your VS Code terminal.

Example:
```bash
wget -O - https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
```

### Install jupyter notebook:
```bash
pip install jupyter notebook
```
Then run:
```bash
jupyter notebook
```
to find the port or URL to the jupyter notebook which can be accessed by copying the url which is given after running the command.