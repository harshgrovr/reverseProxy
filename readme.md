### We are running flask or streamlit basic app:

#### We are running an apache server and streamlit installed, make sure you install apache server:

[Install apache](https://www.cherryservers.com/blog/how-to-install-and-configure-apache-reverse-proxy-server-with-ssl-encryption)

#### Make sure apache2 is running 

```
sudo systemctl status apache2
```


#### and the conf file, in the repo you will find, you move it to following location:

```
/etc/apache2/sites-available/cherry.conf
```

#### Restart the apache2 server:

```
sudo systemctl restart apache2
```


#### Now run flask server from inside the git repo, command to run flask :


```
export FLASK_APP=flask_app.py

flask run --port=8080
```
#### stop the flask server and start the streamlit server from inside the repo:

```
streamlit run flask_app.py
```



