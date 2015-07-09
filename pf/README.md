Docker container for running my personal-financier application.

To build this container: 
`sudo docker build -t malone-cloud/pf .`

To run this container:
`sudo docker run --rm -it -p 80:8080 malone-cloud/pf -e PF_MYSQL_DB_USERNAME=username -e PF_MYSQL_DB_PASS=pass -e PF_MYSQL_DB_URL=mysqldburljdbc:mysql://localhost:3306/dbname`
