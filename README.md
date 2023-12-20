Basic Templates. Feel free to use and modify.

Wazuh template:
You need userparamater for zabbix agent. Tested on Zabbix V6.
        userparameter:
        
        cat /etc/zabbix/zabbix_agentd.d/wazuh-status.conf 
        UserParameter=wazuh.status, curl -s -k -XGET -u username:password 'https://127.0.0.1:9200/_cluster/health?pretty'

        
