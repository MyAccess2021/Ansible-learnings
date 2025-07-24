# **Install Ansible on Ubuntu using Python Virtual Environment**

## **1. Verify Python3 Installation**

```bash
python3 --version
apt install python3-pip
```

---

## **2. Install Python3 if Missing**

```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3
sudo apt install python3-pip
python3 --version
```

---

## **3. Install Dependencies**

```bash
sudo apt-get install python3-minimal python3-virtualenv python3-dev build-essential
```

---

## **4. Set up Virtual Environment**

```bash
mkdir ansible
cd ansible
virtualenv myansible
```

---

## **5. Activate Virtual Environment**

```bash
source myansible/bin/activate
```

---

## **6. Install Ansible**

```bash
pip3 install ansible
```

---

## **7. Verify Ansible Version**

```bash
ansible --version
```
Expected Output
```
ansible [core 2.18.7]
  config file = None
  configured module search path = ['/home/ubuntu/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /home/ubuntu/ansible/myansible/lib/python3.12/site-packages/ansible
  ansible collection location = /home/ubuntu/.ansible/collections:/usr/share/ansible/collections
  executable location = /home/ubuntu/ansible/myansible/bin/ansible
  python version = 3.12.3 (main, Jun 18 2025, 17:59:45) [GCC 13.3.0] (/home/ubuntu/ansible/myansible/bin/python)
  jinja version = 3.1.6
  libyaml = True
```
## If you want to deactivate the virtual environment 
```
deactivate
```
## Check the ansible exist or not in their 
```
ansible --version
```
Expected Output
```
Command 'ansible' not found, but can be installed with:
sudo apt install ansible-core
```

## Create the configuration file and bind it
```
touch ./ansible.cfg
```
Expected output 
```
ansible [core 2.18.7]
  config file = /home/ubuntu/ansible/ansible.cfg
  configured module search path = ['/home/ubuntu/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /home/ubuntu/ansible/myansible/lib/python3.12/site-packages/ansible
  ansible collection location = /home/ubuntu/.ansible/collections:/usr/share/ansible/collections
  executable location = /home/ubuntu/ansible/myansible/bin/ansible
  python version = 3.12.3 (main, Jun 18 2025, 17:59:45) [GCC 13.3.0] (/home/ubuntu/ansible/myansible/bin/python)
  jinja version = 3.1.6
  libyaml = True
```

---

✅ **Ansible installation completed successfully inside a virtual environment.**

---
