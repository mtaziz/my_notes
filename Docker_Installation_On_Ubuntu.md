# my_notes

### Docker Installation on Ubuntu Step 1 ###
Source: [digital ocean](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-14-04)

    wget -qO- https://get.docker.com/ | sh
    sudo usermod -aG docker $(whoami)

### Step 2: Install  Docker-Compose ###

    sudo apt-get -y install python-pip
    # Don't use sudo when installing python-pip, I have already installed pip so I don't need to install**
    pip install docker-compose



### My Docker ###

    mkdir docker-projects
    mkdir hello-world
    cd hello-world
    vim docker-compose.yml
    
### 
    
### Google Chrome Duplicates source Removal ### 

    grep -R --include="*.list" chrome /etc/apt/
    sudo vim /etc/apt/sources.list
    # disable the link & save
### Sample Docker image ###

**compose-docker.yml

    my-test:
        image: hello-world

### Run the command ### 

    docker-compose up

NOTE: I had issues when  command of `docker-compose up` executed but there was sort of permision issues. 
I did not use ` sudo apt-get install python-pip` as I had `pip` previously installed. 
In virtualenv, I installed pip without using sudo. Therefore, I installed *docker-compose* using `pip install docker-compose`.
Then I had to restart the machine. 




