## Profesor: Edwin Montoya, Universidad EAFIT, Medellín-Colombia
## emontoya@eafit.edu.co

# primeros pasos con ElasticSearch - webinar:

https://www.elastic.co/es/webinars/getting-started-logstash

# instalar:

    AWS EC2: t2.large / 20 GB DD

    wget https://artifacts.elastic.co/downloads/logstash/logstash-8.15.3-linux-x86_64.tar.gz

    tar -xzf logstash-8.15.3-linux-x86_64.tar.gz

    cd logstash-8.15.3

    bin/logstash -f etl-file.conf