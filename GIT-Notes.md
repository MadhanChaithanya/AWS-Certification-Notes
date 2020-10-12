# Version Controlling:

* All the team members upload their code into a remote server which is called as __code repository__ or a __Version Controlling System__.
* This Version Controling System accepts the code uploads from multiple team members and it integrates the code into a single projects.
* Next time, when the team members download the code they will be able to access not only their code, but also the code created by the entire team members.

* VCS's preserve older and later versions of the code, so that the team members can toggle between what ever version they want.

* VCS's keep a track of who is making what kind of changes at what time.

#### VCS's are classified  into 2 types:
    1) Centralized Version Controlling.
    2) Distributed Version Controlling.

### 1) Centralized Version Controlling:
* Here we have a remote server where version controlling is done.
* All the team members simply upload their code(Check-in) into this remote servers.
    * Eg: SVN is used for Centralized Version Controlling.
    ![Preview](./Images/1.jpg)    

### 2) Distributed Version Controlling:
* Here we have a local repository on every team members machine where the code is commited into and in the local repository. 
* In the local repository Version controlling happen at the level of the individual team member.
* Later this can be checked-in into a remote server where version controlling happens at the level of the entire team.
    Eg: GitHub is used for Distributed Version Controlling.
    ![Preview](./Images/2.jpg)

For GitHub Installation and Configuration follow the Link here:
![https://www.youtube.com/watch?v=RfrAVPGo5Do&t=94s]

#### Installing Git on Ubuntu:
1. Open terminal in Ubuntu
2. Update the apt repository 
    ```
    sudo apt-get update
    ```
   
3. Install git
    ```
    sudo apt-get install -y git
    ```

#### Installing RHEL, CentOS on Ubuntu:
1. Open terminal in Ubuntu
2. Update the yum repository 
    ```
    yum -y update
    ```
   
3. Install git
    ```
    yum install -y git
    ```

#### Setting up the User name and email globally for all users on a specific machine:
    ```
    git config --global user.name "ChaithanyaGVSM"
    git config --global user.email "gvsmchaithanya@gmail.com"
    ```

#### To see the list of configuration on git:
    ```
    git config --global --list
    ```