1. export $(grep -v '^#' .env | xargs) to export variables
2. in my_config_folder, manage the pipeline.yml (would be called by logstash)
3. launch logstash using my_config_folder : /home/remi/Documents/ansible/ansible_incident/roles/logstash/vars/logstash-8.4.1/bin/logstash --path.settings $LS_SETTINGS_DIR 

KEYSTORE:
1.  sudo ~/Documents/ansible/ansible_incident/roles/logstash/vars/logstash-8.4.1/bin/logstash-keystore create --path.settings $LS_SETTINGS_DIR

2. sudo  ~/Documents/ansible/ansible_incident/roles/logstash/vars/logstash-8.4.1/bin/logstash-keystore add timing --path.settings $LS_SETTINGS_DIR

3. prompt linux....

4. Check with sudo ~/Documents/ansible/ansible_incident/roles/logstash/vars/logstash-8.4.1/bin/logstash-keystore list --path.settings $LS_SETTINGS_DIR

