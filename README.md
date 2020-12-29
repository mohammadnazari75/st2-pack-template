[![StackStorm](https://github.com/stackstorm/st2/raw/master/stackstorm_logo.png)](http://www.stackstorm.com)

# ST2 Installation and ChatOps Configuration
[Ansible and ChatOps. Get started 🚀](https://stackstorm.com/2015/06/24/ansible-chatops-get-started-%F0%9F%9A%80/)

## ST2 Installation with Ansible
[Ansible-ST2](https://github.com/stackstorm/ansible-st2)

## Configure ChatOps
You should configure Slack and Bot configuration in `/opt/stackstorm/chatops/st2chatops.env`

## Configuration

Now if you want to run an action in Slack, you should create a `yaml` file in `actions` and `aliases`.

## Actions
Action files is the action that you want to take through the st2 and for example running a playbook. so create a file same as the other ones and address the ansible playbook.

## Aliases
Aliases file is the way of communicating with Slack. The way of representing the data to st2 and also how to return answer for successes and failures.

> After writing your files, you should install new actions and aliases into the server using this command: `sudo st2 pack install mohammadnazari75/st2-pack-template`

Now you can test your action and alias through slack.
