# Ansible Automated HAProxy Load Balancer Project
![Running GIF](https://camo.githubusercontent.com/1140a4f2ffe1d7d5432df78421909e56c97909423568e609983ec3d4fbcb0b22/68747470733a2f2f726561646d652d747970696e672d7376672e6865726f6b756170702e636f6d3f666f6e743d4f72626974726f6e2673697a653d343026636f6c6f723d253233373941353030266865696768743d3637266475726174696f6e3d333030302663656e7465723d74727565266c696e65733d254630253946253835254236254630253946253836253831254630253946253835254234254630253946253835254234254630253946253836253833254630253946253835254238254630253946253835254244254630253946253835254236254630253946253836253832)


Welcome to the Ansible Automated HAProxy Load Balancer project! This project aims to provide a simplified and beginner-friendly approach to setting up an automated HAProxy load balancer using Ansible.

## Project Overview

- This project involves an Ansible controller node and three managed nodes (two servers and one load balancer).
- The files in this repository are designed to be used on the Ansible controller node, with the `hosts` file located at `/etc/ansible/`.
- By running the `web.yml` Ansible playbook, the managed nodes are configured as PHP servers.
- Running the `lb.yml` playbook sets up the load balancer on port 8080 for distributing client requests.

## Usage Steps

1. Make sure to update the `hosts` file with the public IPs of your instances.
2. In the `hosts` file, place the IP of the load balancer under the `[lb]` group, and the IPs of the server computers under the `[web]` group.
3. You can add as many servers as needed for load balancing, but only one load balancer can be added.
4. Ensure that all managed Ansible nodes can be connected via SSH to the Ansible controller node.

## Notes and Recommendations

- This project has been tested on AWS cloud.
- If you encounter any issues, feel free to contact me at iambhavishyasharma@gmail.com.

This project aims to provide clarity and simplicity, especially for beginners who are new to Ansible and load balancing concepts.

Thank you for using this project! Enjoy your automated HAProxy load balancer setup.
![Running GIF](  https://raw.githubusercontent.com/trinib/trinib/82213791fa9ff58d3ca768ddd6de2489ec23ffca/images/footer.svg)
