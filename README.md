# STOR - Save The Onion Router

As I understand that not all people can afford to configure such a relay (for reasons of lack of competence, desire, time, or jurisdictional difficulties), I recently launched [SaveTor.network](https://savetor.network/), a fundraising campaign to configure and manage new guard/middle relays.

While starting and running new nodes, I realized that I needed a kind of tool that would automate most of my processes, and that would probably have helped a huge slice of the public who would like to launch a new node; but who does not have the skills to do it in simplicity and safety.
If you plan to run more than a single relay, or you want to run a high capacity relay (multiple Tor instances per server) or want to use strong security features like Offline Master Keys without performing additional steps manually, you may want to use configuration management for better maintainability.

The following tutorial and Ansible Role has specifically been built for Tor relay operators and supports multiple operating systems: Ansible Relayor.

## Ansible

[Ansible](https://www.ansible.com/) is an IT automation tool. It can configure systems, deploy software, and orchestrate more advanced IT tasks such as continuous deployments or zero downtime rolling updates.

Ansible’s main goals are simplicity and ease-of-use. It also has a strong focus on security and reliability, featuring a minimum of moving parts, usage of OpenSSH for transport (with other transports and pull modes as alternatives), and a language that is designed around auditability by humans–even those not familiar with the program.

We believe simplicity is relevant to all sizes of environments, so we design for busy users of all types: developers, sysadmins, release engineers, IT managers, and everyone in between. Ansible is appropriate for managing all environments, from small setups with a handful of instances to enterprise environments with many thousands of instances.

Ansible manages machines in an agent-less manner. There is never a question of how to upgrade remote daemons or the problem of not being able to manage systems because daemons are uninstalled. Also, security exposure is greatly reduced because Ansible uses OpenSSH — the open source connectivity tool for remote login with the SSH (Secure Shell) protocol.

Ansible is decentralized–it relies on your existing OS credentials to control access to remote machines.
