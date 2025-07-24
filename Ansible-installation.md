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

---

✅ **Ansible installation completed successfully inside a virtual environment.**

---
