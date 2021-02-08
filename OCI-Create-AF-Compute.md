# Create a Compute instance

An Oracle Compute instance is a Cloud VM that you will use to install and run all of the software for the lab.  

1. Click "Create a VM instance" in the Compute box.
   ![OCI Cloud Dashboard](https://osblaineora.github.io/cicd-tools-db-dev/images/cloudDashboard.png)
1. Populate the name or keep the default.
   ![Create Compute instance form](https://osblaineora.github.io/cicd-tools-db-dev/images/createComputeForm1.png)
1. Scroll down the the "Add SSH keys" section.
1. Select "Paste SSH keys".
1. In your **Cloud Shell**
   1. Generate a new RSA key pair.

      ```bash
      ssh-keygen -t rsa -N "" -b 2048 -C "cloud_shell" -f ~/.ssh/id_rsa
      ```

   1. Display the public key and copy it.

      ```bash
      cat ~/.ssh/id_rsa.pub
      ```

1. In the **Create Compute form**, paste the public key in the SSH KEYS box.
   ![Create Compute instance form](https://osblaineora.github.io/cicd-tools-db-dev/images/createComputeForm2.png)
   If you intend to SSH into your compute instance from any other machine, you may click the "+ Another Key" button and enter the public key for that machine.  
   (you may also want to save a copy of the Cloud Shell private key '~/.ssh/id_rsa' on your local machine.)  
   **DO NOT SHARE your private key**.  This key allows access to your compute instance.
1. Click "Create".
