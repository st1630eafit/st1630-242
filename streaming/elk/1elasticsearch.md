## Profesor: Edwin Montoya, Universidad EAFIT, Medellín-Colombia
## emontoya@eafit.edu.co

# primeros pasos con ElasticSearch - webinar:

https://www.elastic.co/es/webinars/getting-started-elasticsearch

datos para el ejercicio en Kibana/Dev Tools:
    https://assets.contentstack.io/v3/assets/bltefdd0b53724fa2ce/blt56ad3f4e2c755f29/5d37c1602a506857d64eff48/es_commands.txt
    
# instalar:

    AWS EC2: t2.large / 20 GB DD (si va a usar API REST remoto, recuerde abrir el puerto 9200 y verificar que esta 'oyendo' o listing por 0.0.0.0)
    wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.15.3-linux-x86_64.tar.gz
    
    tar -xzf elasticsearch-8.15.3-linux-x86_64.tar.gz

    cd elasticsearch-8.15.3/

# iniciar servidor:

    bin/elasticsearch -d -p pid

# cambiar este settings (una sola vez):
    nano  config/elasticsearch.yml
and replace this setting with false

    xpack.security.enabled: false

# terminar:

    pkill -F pid