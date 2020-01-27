# Simple-REST-API-in-PHP
https://www.codeofaninja.com/2017/02/create-simple-rest-api-in-php.html

## database queries (PostgreSQL)

(two missing queries at start)

CREATE TABLE IF NOT EXISTS products (
  id int NOT NULL DEFAULT nextval('table_name_id_seq'::regclass),
  name varchar(32) NOT NULL,
  description text NOT NULL,
  price decimal(10,0) NOT NULL,
  category_id int NOT NULL,
  created date NOT NULL,
  modified timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
  PRIMARY KEY (id)
)
