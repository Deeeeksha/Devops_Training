
#### Question/Answers

### 1- Is ansible mutable or immutable ? 
Ans.Ansible is a mutable infrastructure.Ansible does have the ability to provision cloud infrastructure as well, but its procedural nature makes it ill suited to large infrastructure deployments.

### 2- What do you mean by provisioning in ansible?
Ans. Creating a suitable environment for the application/ software to live is necessary. Ansible provides a way to automate the environment created for the application's existence.

### 3- What is configuration management ? 
Ans. Ansible is a configuration management platform that automates storage, servers, and networking. When you use Ansible to configure these components, difficult manual tasks become repeatable and less vulnerable to error.

### 4- What is a public and private cloud ?
Ans. Public cloud is cloud computing that's delivered via the internet and shared across organizations. Private cloud is cloud computing that is dedicated solely to your organization. Hybrid cloud is any environment that uses both public and private clouds.Private cloud is also known as an internal cloud or corporate cloud. Private cloud provides computing services to a private internal network (within the organization) and selected users instead of the general public

### 5- What is Inventory? 
Ans. The Ansible inventory file defines the hosts and groups of hosts upon which commands, modules, and tasks in a playbook operate. The file can be in one of many formats depending on your Ansible environment and plugins.

### 6- What is idempotency in ansible? 
Ans. A principle that enables Ansible to be declarative & reliable is idempotence. For Ansible it means after 1 run of a playbook to set things to a desired state, further runs of the same playbook should result in 0 changes. In simplest terms, idempotency means you can be sure of a consistent state in your environment.

### 7- What is CMDB ?
Ans. CMDB stands for Configuration Management Database . Ansible-cmdb takes the output of Ansible's fact gathering and converts it into a static HTML overview page (and other things) containing system configuration information. It supports multiple types of output (html, csv, sql, etc) and extending information gathered by Ansible with custom data.

### 8- Learn about plugins
Ans. Plugins are pieces of code that augment Ansible's core functionality. Ansible uses a plugin architecture to enable a rich, flexible and expandable feature set. Ansible ships with a number of handy plugins, and you can easily write your own.

### 9- How ansible connects to the localhost ?
Ans.Ansible connects to the localhost as:

Method1:  Specify Localhost in your hosts directive of your playbook.

Method2:  Using local_action clause in the ansible playbook.

Method3:  Add an entry in your Inventory.

Method4:  Specify in the Ansible Command line.


### 10 - How can you remove or uninstall an application completely on the host machine ?
Ans. This can be done as:    
              
              $ sudo apt-get remove package-name

               $ sudo apt-get purge package-name
 
               $ sudo apt-get autoremove: to remove any dependencies such as the applications and libraries used by the software


### 11- If the host machine does not have python then how will you install python on it using ansible?
Ans. By using the raw module. It executes a low-down and dirty SSH command.Note: If using raw from a playbook, you may need to disable fact gathering using gather_facts:
no if you’re using raw to bootstrap python onto the machine.bc  

### 12- What is the role of  networking in Ansible ?
Ans. Ansible Network modules extend the benefits of simple, powerful, agentless automation to network administrators and teams. Ansible Network modules can configure your network stack,
test and validate existing network state, and discover and correct network configuration drift.Because the majority of network devices can not run Python, the Ansible network modules are
executed on the Ansible control node, where ansible or ansible-playbook runs. Network modules also use the control node as a destination for backup files, for those modules that offer a backup option.
