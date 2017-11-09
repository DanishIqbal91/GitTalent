# Couchbase GitTalent Demo

This repository contains all the code for the GitTalent application built for Couchbase Connect 2016 Keynote demo.

[![Keynote: Beyond NoSQL – Building a digital future – Couchbase Connect 2016](https://img.youtube.com/vi/Bq8zkcbnRac/0.jpg)](https://youtu.be/Bq8zkcbnRac?t=1579) 


We wrote [a guide](./GitTalent.asciidoc) explaining every development step we went through to build this application.

[Installation instructions](./INSTALL.md) are available as well.


jenkins
in build section

cd gittalent-frontend
npm install
ng build
sudo docker build -t frontend .

in Post build section
#sudo docker rm -f angular || true
sudo docker run -d -p 804:80 --name angular8 frontend
