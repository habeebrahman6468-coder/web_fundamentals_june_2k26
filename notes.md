### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`

url:localhost:8000/movie/
method:POST
body{"title":"kgf",
      "year":2008,
      "language":"kannada"
      "run_time":160}

      
`http_request for list all movie`

url:localhost:8000/movie/
method:GET


`http_request for fetching movie detail`

url:localhost:8000/movie/1/
method:GET

`http_request for update movie`

url:localhost:8000/movie/5/
method:PUT
body{"title":"BKD",
     "year":2026,
     "language":"malayalam,
     "run_time":150,
     }


`http_request for delete movie`

url:localhost:8000/movie/2/
method:DELETE


### Hospital Task

'''
patients

patient_id  patient_name   assigned_doctor  department        appointment_date     status      consultation_fee     

1           Arun           Dr Rajesh        Dermatology       2026-09-10           pending     500             
2           Sneha Nair     Dr Meera         General Medicine  2026-09-11           completed   700          
3           Anjali Menon   Dr Priya         cardiology        2026-09-12           pending     400
4           vishnu         Dr Anil          orthopaedics      2026-09-14           pending     300
5           Rahul das      Dr Suresh        paediatrics       2026-09-15           completed   350


`http_request for adding new patient`

url:localhost:8000/patients/
method:POST
body{"patient_name":"Arun",
        "assigned_doctor":"Dr Rajesh",
        "department":"Dermatology",   
        "appointment_date":20206-09-10,  
        "status":"pending",  
        "consultation_fee":500
    }

`http_request for list all patient`

url:localhost:8000/patients/
method:GET

`http_request for fetching patient detail`

url:localhost:8000/patients/3/
method:GET

`http_request for update patient`

url:localhost:8000/patients/4/
method:PUT
body{"patient_name":"Anjali menon",
        "assigned_doctor":"Dr Priya",
        "department":"Cardiology",   
        "appointment_date":20206-09-12,  
        "status":"pending",  
        "consultation_fee":400
    }

`http_request for delete movie`

url:localhost:8000/patients/5/
method:DELETE

