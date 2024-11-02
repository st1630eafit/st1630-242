## Profesor: Edwin Montoya, Universidad EAFIT, Medellín-Colombia
## emontoya@eafit.edu.co

# instalar:

    AWS EC2: t2.large / 20 GB DD

Filebeat: https://www.elastic.co/es/downloads/beats/filebeat (envio de logs de una máquina Linux a ElasticSearch)

    wget https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-8.15.3-linux-x86_64.tar.gz

    tar -xzf filebeat-8.15.3-linux-x86_64.tar.gz
    cd filebeat-8.15.3-linux-x86_64

Edit the filebeat.yml configuration file
Start the daemon by running:

este ejemplo envia todos los logs de: /var/log/*.log

    sudo chown root filebeat.yml
    sudo ./filebeat -e -c filebeat.yml

Metricbeat: https://www.elastic.co/es/downloads/beats/metricbeat (envio de info del sistema - cpu, mem, disco, etc a ElasticSearch)

    wget https://artifacts.elastic.co/downloads/beats/metricbeat/metricbeat-8.15.3-linux-x86_64.tar.gz

    tar -xvf metricbeat-8.15.3-linux-x86_64.tar.gz
    
    cd metricbeat-8.15.3-linux-x86_64

Edit the metricbeat.yml configuration file:

    sudo ./metricbeat -e -c metricbeat.yml