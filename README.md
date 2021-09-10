# Software Acrhitectures

This project is created for final exam for Advanced Software Architectures.

It consists of two applications, front end and backend. App is made for managing employees and departments inside one organization.

Frontend app is done in react and backend are done in Spring Boot. Backend consist of four microservices, one is Discovery service and the other three and made as clients.

## Organization service

Get all organizations - GET
```
http://localhost:9003/
```

Add ogranization - POST - params: organization
```
http://localhost:9003/
```

Get specific organization - GET
```
http://localhost:9003/{id}
```

Update specific organization - PUT - params: id, organization
```
http://localhost:9003/{id}
```

Delete specific organization - DELETE - params: organization id (deletes all departmets and employees too)
```
http://localhost:9003/{id}
```

Get specific organization with departments - GET
```
http://localhost:9003/{id}/with-departments
```

Get specific organization with employees - GET
```
http://localhost:9003/{id}/with-employees
```

Get specific organization with departments and employees - GET
```
http://localhost:9003/{id}/with-departments-and-employees


## Department service


Get all departments - GET
```
http://localhost:9002/
```

Add department - POST - params: department
```
http://localhost:9002/
```

Get specific department - GET
```
http://localhost:9002/{id}
```

Update specific department - PUT - params: id, department
```
http://localhost:9002/{id}
```

Delete specific department - DELETE - params: department id (deletes employees too)
```
http://localhost:9002/{id}
```

Get all departments by organization id - GET
```
http://localhost:9002/organization/{organizationId}
```

Delete all departments by organization id - DELETE - params : organization id (deletes employees too)
```
http://localhost:9002/organization/{organizationId}
```

Get specific department with employees - GET
```
http://localhost:9002/{id}/with-employees
```

Get departments with employees by organization id - GET
```
http://localhost:9002/organization/{organizationId}/with-employees"
```

## Employee service

Get all employees - GET
```
http://localhost:9001/
```

Add employee - POST - params: employee
```
http://localhost:9001/
```

Get specific employee - GET
```
http://localhost:9001/{id}
```

Update specific employee - PUT - params: id, employee
```
http://localhost:9001/{id}
```

Delete specific employee - DELETE - params: id 
```
http://localhost:9001/{id}
```

Get all employees by organization id - GET
```
http://localhost:9001/organization/{organizationId}
```

Delete all employees by organization id - DELETE - params : organization id 
```
http://localhost:9001/organization/{organizationId}
```


Get all employees by department id - GET
```
http://localhost:9001/department/{departmentId}
```

Delete all employees by department id - DELETE - params : department id 
```
http://localhost:9001/department/{departmentId}
