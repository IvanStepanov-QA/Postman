### Postman.
# __HW_1__

_Создать запросы в Postman._

- Protocol: http
- IP: 162.55.220.72
- Port: 5005

__EP_1__
- Method: GET
- EndPoint: /get_method
- request url params: 
 - name: str
 - age: int

==================

__EP_2__
- Method: POST
- EndPoint: /user_info_3
- request form data: 
 - name: str
 - age: int
 - salary: int

- response: 

		{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}


==================

__EP_3__
- Method: GET
- EndPoint: /object_info_1
- request url params: 
 - name: str
 - age: int
 - weight: int

        response: 
        {'name': name,
                  'age': age,
                  'daily_food': weight * 0.012,
                  'daily_sleep': weight * 2.5}


==================

__EP_4__
- Method: GET
- EndPoint: /object_info_2
- request url params: 
 - name: str
 - age: int
 - salary: int

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


==================

__EP_5__
- Method: GET
- EndPoint: /object_info_3
- request url params: 
 - name: str
 - age: int
 - salary: int

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


==================

__EP_6__
- Method: GET
- EndPoint: /object_info_4
- request url params: 
 - name: str
 - age: int
 - salary: int

        response: 
        {'name': name,
                  'age': int(age),
                  'salary': [salary, str(salary * 2), str(salary * 3)]}


==================

__EP_7__
- Method: POST
- EndPoint: /user_info_2
- request form data: 
 - name: str
 - age: int
 - salary: int

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

# __HW_2__

http://162.55.220.72:5005/first
1. Отправить запрос.
2. Статус код 200
3. Проверить, что в body приходит правильный string.

http://162.55.220.72:5005/user_info_3
1. Отправить запрос.
2. Статус код 200
3. Спарсить response body в json.
4. Проверить, что name в ответе равно name из request (name вбить руками.)
5. Проверить, что age в ответе равно age из request (age вбить руками.)
6. Проверить, что salary в ответе равно salary из request (salary вбить руками.)
7. Спарсить request.
8. Проверить, что name в ответе равно name из request (name забрать из request.)
9. Проверить, что age в ответе равно age из request (age забрать из request.)
10. Проверить, что salary в ответе равно salary из request (salary забрать из request.)
11. Вывести в консоль параметр family из response.
12. Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)

http://162.55.220.72:5005/object_info_3
1. Отправить запрос.
2. Статус код 200
3. Спарсить response body в json.
4. Спарсить request.
5. Проверить, что name в ответе равно name из request (name забрать из request.)
6. Проверить, что age в ответе равно age из request (age забрать из request.)
7. Проверить, что salary в ответе равно salary из request (salary забрать из request.)
8. Вывести в консоль параметр family из response.
9. Проверить, что у параметра dog есть параметры name.
10. Проверить, что у параметра dog есть параметры age.
11. Проверить, что параметр name имеет значение Luky.
12. Проверить, что параметр age имеет значение 4.


============================================================================
http://162.55.220.72:5005/object_info_4
1. Отправить запрос.
2. Статус код 200
3. Спарсить response body в json.
4. Спарсить request.
5. Проверить, что name в ответе равно name из request (name забрать из request.)
6. Проверить, что age в ответе равно age из request (age забрать из request.)
7. Вывести в консоль параметр salary из request.
8. Вывести в консоль параметр salary из response.
9. Вывести в консоль 0-й элемент параметра salary из response.
10. Вывести в консоль 1-й элемент параметра salary параметр salary из response.
11. Вывести в консоль 2-й элемент параметра salary параметр salary из response.
12. Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)
13. Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)
14. Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)
15. Создать в окружении переменную name
16. Создать в окружении переменную age
17. Создать в окружении переменную salary
18. Передать в окружение переменную name
19. Передать в окружение переменную age
20. Передать в окружение переменную salary
21. Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.

=============================================================================

http://162.55.220.72:5005/user_info_2
1. Вставить параметр salary из окружения в request
2. Вставить параметр age из окружения в age
3. Вставить параметр name из окружения в name
4. Отправить запрос.
5. Статус код 200
6. Спарсить response body в json.
7. Спарсить request.
8. Проверить, что json response имеет параметр start_qa_salary
9. Проверить, что json response имеет параметр qa_salary_after_6_months
10. Проверить, что json response имеет параметр qa_salary_after_12_months
11. Проверить, что json response имеет параметр qa_salary_after_1.5_year
12. Проверить, что json response имеет параметр qa_salary_after_3.5_years
13. Проверить, что json response имеет параметр person
14. Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)
15. Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)
16. Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)
17. Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)
18. Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)
19. Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)
20. Проверить, что что параметр u_age равен age из request (age забрать из request.)
21. Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)
22. ***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.

# __HW_3__  
=====

1) необходимо залогиниться
<br>POST
<br>http://162.55.220.72:5005/login
<br>login : str (кроме /)
<br>password : str

Приходящий токен необходимо передать во все остальные запросы.

===================
- дальше все запросы требуют наличие токена.

===================

2) ___http://162.55.220.72:5005/user_info___
<br>req. (RAW JSON)
<br>POST
<br>age: int
<br>salary: int
<br>name: str
<br>auth_token


          resp.
          {'start_qa_salary':salary,
           'qa_salary_after_6_months': salary * 2,
           'qa_salary_after_12_months': salary * 2.9,
           'person': {'u_name':[user_name, salary, age],
                                          'u_age':age,
                                          'u_salary_1.5_year': salary * 4}
                                          }

Тесты:
1) Статус код 200
2) Проверка структуры json в ответе.
3) В ответе указаны коэффициенты умножения salary, напишите тесты по проверке правильности результата перемножения на коэффициент.
4) Достать значение из поля 'u_salary_1.5_year' и передать в поле salary запроса http://162.55.220.72:5005/get_test_user 

===================

3. ___http://162.55.220.72:5005/new_data___
<br>req.
<br>POST
<br>age: int
<br>salary: int
<br>name: str
<br>auth_token

Resp.

    {'name':name,
      'age': int(age),
      'salary': [salary, str(salary*2), str(salary*3)]}

Тесты:
1) Статус код 200
2) Проверка структуры json в ответе.
3) В ответе указаны коэффициенты умножения salary, напишите тесты по проверке правильности результата перемножения на коэффициент.
4) проверить, что 2-й элемент массива salary больше 1-го и 0-го

===================

4) ___http://162.55.220.72:5005/test_pet_info___
<br>req.
<br>POST
<br>age: int
<br>weight: int
<br>name: str
<br>auth_token


<br>Resp.

    {'name': name,
     'age': age,
     'daily_food':weight * 0.012,
     'daily_sleep': weight * 2.5}


Тесты:
1) Статус код 200
2) Проверка структуры json в ответе.
3) В ответе указаны коэффициенты умножения weight, напишите тесты по проверке правильности результата перемножения на коэффициент.

===================

5) ___http://162.55.220.72:5005/get_test_user___
<br>req.
<br>POST
<br>age: int
<br>salary: int
<br>name: str
<br>auth_token

<br>Resp.

    {'name': name,
     'age':age,
     'salary': salary,
     'family':{'children':[['Alex', 24],['Kate', 12]],
     'u_salary_1.5_year': salary * 4}
      }

Тесты:
1) Статус код 200
2) Проверка структуры json в ответе.
3) Проверить что занчение поля name = значению переменной name из окружения
4) Проверить что занчение поля age в ответе соответсвует отправленному в запросе значению поля age

===================
