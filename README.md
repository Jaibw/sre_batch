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
