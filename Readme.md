# AIoT Github

## Lecture 15: IoT Flask Web (deploy to heroku)

### step 1 : Clone this github

### step 2 : install some package

gunicorn 只適用UNIX系統
且本作業好像也用不到?

```python
Flask==2.0.1 
Jinja2==3.0.1 
psycopg2 
sklearn 
pandas  
numpy 
```

### step 3: add an heroku postgredb

* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb

![step3](img/step3.png)

### step 4: login to heroku pstgredb using HeidiSQL

![step4_1](img/step4_1.png)

![step4_2](img/step4_2.png)


### step 5: import postgredb (in db/postgre.sql)

在public資料庫匯入postgre.sql表格

![step5_1](img/step5_1.jpg)

![step5_2](img/step5_2.jpg)

![step5_3](img/step5_3.jpg)

### step 6: setting db in app.py

```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```

![step6](img/step6.png)


### step 7: testing locally by running python app.py

![step7_1](img/step7_1.png)

![step7_2](img/step7_2.png)

### step 8: deploy to github

git push to

link: https://github.com/SmallDragon11/aiot0530-start-no-token


### step 9: Heroku deploy from github

![step9](img/step9.png)

### step 10: Complete

mylink: https://myapp0531.herokuapp.com/

### setRandom heroku:
![setRandomsuccessHeroku](img/setRandom_heroku.png)




### callAI heroku:
![callAIsuccessHeroku](img/callAI_heroku.png)




### setRandom Local:
![setRandomsuccessLocal](img/setRandom.png)




### callAI Local:
![callAIsuccessLocal](img/callAI.png)