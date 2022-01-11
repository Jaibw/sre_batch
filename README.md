# Create users 
<pre>
1. Add one file under user/NAME.yaml
2. wget https://raw.githubusercontent.com/Jaibw/sre_batch/main/user/NAME.yaml
3. ansible-playbook  NAME.yaml
</pre>

# Demo Handlers  
<pre>
cd ~/name    # cd ~/jai
wget https://raw.githubusercontent.com/Jaibw/sre_batch/main/demo/ntp.conf
wget https://raw.githubusercontent.com/Jaibw/sre_batch/main/demo/ntp-ubuntu.yaml
ansible-playbook ntp-ubuntu.yaml
</pre>

# Users with Vars  
<pre>
cd ~/name
wget https://raw.githubusercontent.com/Jaibw/sre_batch/main/user-with-vars.yaml
ansible-playbook user-with-vars.yaml -e username=name0001

</pre>

# Users with loop   
<pre>
cd ~/name
wget https://raw.githubusercontent.com/Jaibw/sre_batch/main/loop/users.yaml
ansible-playbook users.yaml
</pre>

# Secure Playbook   
<pre>
cd ~/name
wget https://raw.githubusercontent.com/Jaibw/sre_batch/main/loop/users.yaml
ansible-vault encrypt users.yaml
cat users.yaml
ansible-vault decrypt users.yaml
cat users.yaml
ansible-vault encrypt users.yaml
cat users.yaml
ansible-vault view users.yaml
ansible-vault edit users.yaml
ansible-playbook users.yaml --ask-vault-pass
</pre>
