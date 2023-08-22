# Ansible Automated HAProxy Load Balancer Project
   - [OpenAI Python](https://github.com/openai/openai-python)


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
