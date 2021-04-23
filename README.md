# python-sabpaisa


This package is used to integrate sabpaisa payment gateway with your python application.

## Installation

You can add SabPaisa SDK to your existing React Native project using following npm command: -

```sh
pip install sabpaisa
```

## Example
```
from sabpaisa import main


dic={"username":"nishant.jha_2885","password":"SIPL1_SP2885","API_KEY":"rMnggTKFvmGx8y1z","API_IV":"0QvWIQBSz4AX0VoH","client_code":"SIPL1","email":"kanu0704@gmail.com"}
s = main.Sabpaisa(URLfailure="http://localhost:8080/payment/",URLsuccess="http://localhost:8080/payment/",payerFirstName="kanishk",payerLastName="kanishk",auth=True,payerContact="+918979626196",payerAddress="ABC",tnxId="32cs42324csvcssdsdd2323",username=dic["username"],password=dic["password"],authKey=dic["API_KEY"],authIV=dic["API_IV"],clientCode=dic["client_code"],payerEmail="kanu0704@gmail.com",txnAmt="400")


print(s.genrateLink())
```





## License

MIT
