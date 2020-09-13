Technolgy used: Java11, SpringBoot, 
Database : Postgres
Find below API Endponts

-----------------------------------------------------------------
1) Create:

	http://localhost:8080/organisation/employee/skill
	
	Headers :
			Key : Content-Type 
			Value : application/json

Method: POST

	Body:
	{
		"user_id":"E003",
		"user_name":"Vishruth",
		"skill_id":"MS001",
		"skills":"C#",
		"proficiency":"3-Expert",
		"effective_date":"2020-09-13T01:14:25.000+0000"
	}
2) Read 
	http://localhost:8080/organisation/employee/skill
		Headers :
			Key : Content-Type 
			Value : application/json

		Method: GET
3) Read (getBySkillName)
	http://localhost:8080/organisation/employee/skill/{skillName}
	http://localhost:8080/organisation/employee/skill/JAVA
	Headers :
			Key : Content-Type 
			Value : application/json

		Method: GET
4) Delete the record
	http://localhost:8080/organisation/employee/{id}
	http://localhost:8080/organisation/employee/105
	Headers :
			Key : Content-Type 
			Value : application/json

		Method: DELETE
5) Update the record
	http://localhost:8080/organisation/employee/{id}
	http://localhost:8080/organisation/employee/105
	Headers :
			Key : Content-Type 
			Value : application/json

		Method: PUT
		Body:
		{
        "id": 105,
        "user_id": "E001",
        "user_name": "Narayanan",
        "skill_id": "J001",
        "skills": "JAVA",
        "proficiency": "1-Expert",
        "effective_date": "2020-09-12T10:03:06.167+0000",
        "create_date": "2020-09-12T10:03:06.167+0000",
        "update_date": "2020-09-12T10:03:06.167+0000"
		}
