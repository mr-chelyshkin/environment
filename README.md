# environment


golang - закидывать в папку tmp

ansible-playbook -i hosts raspberry_devel.yml --user "igoss" --extra-vars "ansible_become_pass=qwerty" --extra-vars "ansible_ssh_pass=qwerty" --extra-vars "ansible_host=igoss.local" --extra-vars "ansible_user=igoss" --extra-vars "pub_key_name=mr_chelyshkin.pub" --extra-vars "private_key_name=mr_chelyshkin"