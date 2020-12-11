# Quiz 2.1

## How to create an Ansible Configuration

1. Check if ansible was installed on your machine using `ansbile --version`. If its installed proceed to `Step 2`. If not use the command `apk add ansible` if you are using Alpine. `apt install ansible` if you are using ubuntu.

2. Create configuration file using the `touch <filename.cfg>` and if yo uwant to edit it use `vim <filename.cfg>`.

3. After you create a configuration file, inside of it add the content or information that you need the `defaults` i.e `remote machine`, `inventory`, `remote_machine`, `remote user` and `privilege escalation`.

4. Save it by using `esc` and `:wq!`.


## How to create Ansible Inventory

1. Create the inventory file by using `touch <filename>` if you want to create it and edit it by using `vim <filename>` .

2. Edit the inventory file by inserting the `IP address` that you want to remote.

3. Additional Information for it you can have many Ip address as long as it's in the network. i.e
`[server_name]`
`IP address]
`[server_name_1]`
`IP address`

4. Save the inventory file by using `esc` and `:wq!`.

## Hot to create an Ad-hoc Ansible command with `setup` and `shell` module

1. Use `ls` command to lists all files and directories within the file system and show detailed information about them.

2. To learn more about Ad-hoc use this link: <https://docs.ansible.com/ansible/latest/user_guide/intro_adhoc.html>.

3. Use `ansible all -m ping` if you want to ping the `IP address` of the remote user inside of the `inventory file`. If the configuration of inventroy are done and successfully the output will be `green` and it shows `successful` and `pong`.

4. For more built-in ansible shell modue i.e `ansible all -m shell -a "date". Click this link: <https://docs.ansible.com/ansible/latest/collections/ansible/builtin/shell_moduel.html>.
