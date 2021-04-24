# python-sabpaisa


This package is used to integrate sabpaisa payment gateway with your python application.

## Installation

You can add SabPaisa SDK to your existing python project using following pip command: -

```sh
pip install sabpaisa
```

## Example
```
from sabpaisa import main


dic={"username":"your username","password":"your password","API_KEY":"your api key","API_IV":"your api iv","client_code":"your client code","email":"your email"}
s = main.Sabpaisa(URLfailure="http://localhost:8080/payment/",URLsuccess="http://localhost:8080/payment/",payerFirstName="someone",payerLastName="someone",auth=True,payerContact="+911234567789",payerAddress="ABC",tnxId="32cs42324csvcssdsdd2323",username=dic["username"],password=dic["password"],authKey=dic["API_KEY"],authIV=dic["API_IV"],clientCode=dic["client_code"],payerEmail="kanu0704@gmail.com",txnAmt="400")


print(s.genrateLink())
```





## License

MIT
