## Cloud Formation:
* Consider creating the Following Architecture
![Preview](./CF1.jpg)

* Options are 
    - AWS Console
    - AWS CLI
* Let's assume, I preferred console and created the architecture using UI.
* Next day, I got a request to recreate the same architecture, for this what should be the approach?
* Mostly automation is the Answer and I have a 2 possibilities 
    - Write a Shell script/powershell script using AWS CLI.
    - Write a cloud formation template.
- Let's stick to shell scripts, for these the problems here
    - Difficult to change.
    - When the script runs it is not guaranteed to get the same result.
- Cloud Formation Template:
    - A JSON/YAML file.
    - It is a IAC [Infrastructure As a CODE]with idempotentance.

* Cloudformation template is a JSON/YAML based declarative way of creating the Infrastructure.

## Lab Setup:
- Git for Windows
'''
choco install git -y
'''
- AWS CLI
'''
choco install awscli -y
'''
- Visual Studio Code
'''
choco install vscode
'''
- Cloud Formation Extension

 ### Basic Cloudformation Template:
 