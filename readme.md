1)Run the containers > #docker-compose up -d

2)browse >ip:9200 (u will get login page) and ip:5601 (Kibana server is not ready yet)

3)run command>> # docker-compose exec elasticsearch bash
4)run command>> # bin/elasticsearch-setup-passwords auto

you will get passwords here,  copy it somewhere and save

5)exit the containers #docker-compose down

6)now update the  docker-compose.yml file by putting kibana passowrd (in environment: ELASTICSEARCH_PASSWORD=: put the password for kibana user )

7)Now run the containers #docker-compose up -d

8)browse > ip:9200 (u will get login page)
>> here put login id: "elastic" and password for user elastic: 
>>the text page get opened.

9)browse > ip:5601 (kibana login page will open)
username : "elastic" and password: (password for user elastic)

 
