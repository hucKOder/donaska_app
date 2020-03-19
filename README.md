# Projekt Donaska

## Windows rozbehanie
1. Nainstalovat PostgreSQL 12.2 [https://www.enterprisedb.com/downloads/postgres-postgresql-downloads](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
2. Nainstalovat Python a Anaconda
3. Vytvorit virtualne prostredie Anaconda s Python 3.6.9
```conda create -n donaska python=3.6.9```
4. Aktivovat virtualne prostredie  
```activate donaska```
5. Nainstalovat Python balicky  
```pip install -r requirements.txt```
6. Vytvorit databazu v PostgreSQL, napr. s menom _donaska_
7. Vytvorit premennu prostredia s adresou a menom databazy  
```setx DATABASE_URL TODOTODO```
8. Spustit migracie  
```python manage.py db init```  
```python manage.py db migrate```