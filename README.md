ksys-docker-idempiere
=======================

Base docker image to run iDempiere-KSYS inside Apache Karaf

Usage
-----

To create the image `longnan/ksys-docker-idempiere`, execute the following command on the ksys-docker-idempiere folder:

	docker build --rm -t longnan/ksys-docker-idempiere .
	docker build --rm -t longnan/ksys-docker-idempiere:2.0.20140608 .

To run the image:

	docker run -d --link ksys-postgresql:idempiere-db --name="ksys-idempiere" -p 8181:8181 longnan/ksys-docker-idempiere:2.0.20140608
	docker run -t -i --link ksys-postgresql:idempiere-db --name="ksys-idempiere" -p 8181:8181 longnan/ksys-docker-idempiere:2.0.20140608 /bin/bash

To start the container:	
	docker start ksys-idempiere

	
