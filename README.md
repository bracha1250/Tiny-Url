# Tinyurl
Tinyurl is an url shortener written in Java using Spring Boot and **MongoDB**,
**Redis** and **cassandra** which supports scaling and high availability.

## Technologies
* **Backend**: Spring-boot (java)
* **Database**:
    * **MongoDB** - for storing users and urls data related to them  (total amount of clicks, total amount of clicks per url, etc)
    * **Redis** - for storing and mapping short url to long url (key-value)
    * **Cassandra** - for storing and logging user's activity about url visits (when, which url, who visited etc.)
* **Containerization**: Docker

# Features
* **Short url** - user can create short url for any url
* **Url statistics** - user can see statistics about his urls (total amount of clicks, total amount of clicks per url, etc) via mongodb
* **Url activity** - user can see activity about his urls (when, which url, who visited etc.) via cassandra
