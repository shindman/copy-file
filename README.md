# copy-file
Copy file to remote. Use raw tab.

vim file.yml

---
- name: Copy sshd file
  copy:
    src: /backup/mongodb_sshd_config 
    dest: /etc/sshd/sshd_config
    owner: root
    group: root
    mode: 0644
    backup: yes
