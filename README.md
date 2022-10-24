# Learning Ansible and Git
## 2022-10-24
1. Install Ansible
sudo apt install ansible

1. Setel Repsitori Git
Buat repositori di Github.
Buat satu file : README.md
Isi file dengan keterangan yang diperlukan, kemudian simpan.
git clone (url_repository)

1. Membuat file inventory
cd ansible
vim inventory
Masukkan alamat IP server

vim ansible.cfg
inventory = inventory
private_key_file = (path_ke_file_private_key)

ansible all -m ping
ansible all --list-hosts
ansible all -m gather_facts
ansible all -m gather_facts --limit (ip_address)
