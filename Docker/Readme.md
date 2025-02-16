## Docker installer
This script installs Docker CLI on your Linux (Ubuntu) machine.

### Post install steps
Run the below commands to be able to run docker without using `sudo`.

1. Create the docker group.
    ```
    sudo groupadd docker
    ```
2. Add your user to the docker group.
    ```
    sudo usermod -aG docker $USER
    ```
3. Log out and log back in so that your group membership is re-evaluated or you can also run the following command to activate the changes to groups:
    ```
    newgrp docker
    ```