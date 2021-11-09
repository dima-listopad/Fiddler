## Домашняя работа Fiddler

Protocol: http
IP: 162.55.220.72
Port: 5005
____
Ex_1: 
Method: GET
EndPoint: /get_method
request url params: 
 name: str
 age: int

response: 
[
    “Str”,
    “Str”
]

Task:
Сделать правила:
 ⁃ Подменить url в чтобы в запросе поменялся name которые вы вписали в Postman.
 - Подменить url в чтобы в запросе поменялся age которые вы вписали в Postman. 
![1](https://user-images.githubusercontent.com/88891623/140916974-a0b9bd5d-907e-422b-b354-15b90885fc85.PNG)
____

Ex_2:
Method: POST
EndPoint: /user_info_3
request form data: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}

Task:
Сделать правила:
 ⁃ Подменить тело запроса чтобы поменялся name которые вы вписали в Postman.
 - Подменить тело запроса чтобы поменялся age которые вы вписали в Postman. 
 - Подменить тело запроса чтобы поменялся salary которые вы вписали в Postman. 
 - Подменить тело запроса чтобы удалился age которые вы вписали в Postman.  (Получить 500 код)
 - В ответе поменять children на neighbors. 
 - В ответе поменять значение зарплаты u_salary_1_5_year на другую цифру. 
 - В ответе удалить параметр salary. 
![2](https://user-images.githubusercontent.com/88891623/140916996-a5c98c5a-c2d0-4d44-9399-f0e5bc92dabe.PNG)
____

Ex_3:
Method: GET
EndPoint: /object_info_1
request url params: 
 name: str
 age: int
 weight: int

response: 
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}

Task:
Сделать правила:
 ⁃ Подменить url в чтобы в запросе поменялся name которые вы вписали в Postman.
 - Подменить url в чтобы в запросе поменялся age которые вы вписали в Postman. 
 - Подменить url в чтобы в запросе поменялся salary которые вы вписали в Postman. 
 - Подменить url в чтобы в запросе удалился weight которые вы вписали в Postman.
 - В ответе удалить параметр  daily_food.
 - В ответе поменять значение параметра daily_food на другую цифру. 
 - В ответе переименовать daily_sleep на sleep
 - В ответе поменять значение параметра daily_sleep на другую цифру. 
![3](https://user-images.githubusercontent.com/88891623/140917005-630d6d2d-5337-4059-8d15-9530d01a7d78.PNG)
____

Ex_4:
Method: GET
EndPoint: /object_info_3
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }

Task:
Сделать правила:
 ⁃ Подменить url в чтобы в запросе поменялся name которые вы вписали в Postman.
 - Подменить url в чтобы в запросе поменялся age которые вы вписали в Postman. 
 - Подменить url в чтобы в запросе удалился name которые вы вписали в Postman.
 - В ответе удалить параметр  salary.
 - В ответе поменять значение параметра cat на другой json. 
 - Получить 405 код
![4](https://user-images.githubusercontent.com/88891623/140917017-5eb082db-997b-4f0f-9628-ceabb626d588.PNG)
____

Ex_5:
Method: GET
EndPoint: /object_info_4
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}


Task:
 ⁃ Подменить url в чтобы в запросе поменялся name которые вы вписали в Postman.
 - Подменить url в чтобы в запросе поменялся age которые вы вписали в Postman. 
 - Подменить url в чтобы в запросе удалился salary которые вы вписали в Postman.
 - В ответе удалить параметр  salary.
 - В ответе поменять значение параметра salary на значение текстового типа. 
 - Получить 405 код
![5](https://user-images.githubusercontent.com/88891623/140917035-b9860f81-b6c7-43e7-96bc-723f931f61f3.PNG)
____

Ex_6:
Method: POST
EndPoint: /user_info_2
request form data: 
 name: str
 age: int
 salary: int
response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }


Task:
Сделать правила:
 - Подменить тело запроса чтобы поменялся age которые вы вписали в Postman. 
 - Подменить тело запроса чтобы поменялся salary которые вы вписали в Postman. 
 - Подменить тело запроса чтобы удалился salary которые вы вписали в Postman.
 - В ответе поменять qa_salary_after_6_months на qa_salary_after_10_months. 
 - В ответе поменять значение зарплаты qa_salary_after_1.5_year на другую цифру. 
 - В ответе удалить параметр person. 
 - В ответе поменять значение параметр person с json на xml. 
![6](https://user-images.githubusercontent.com/88891623/140917064-e6f61198-8b36-43f2-91be-56887e473543.PNG)
