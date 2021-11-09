# Getting Started

## 1. Glosary

The following specify terms and abbreviations used in this document and their definitions that are needed to understand this document.
##


Abbreviations |  Definition
:------------ | -------------
SSM | Suruhanjaya Syarikat Malaysia
MB | Mesiniaga Berhad
Hash | Hash is a one way function -it cannot be decrypted back.
SHA | Secure Hash Algorithmis one of a number of cryptographic hash functions.
SHA256 | SHA-256 variant of SHA algorithm generates an almost-unique, fixed size 256-bit(32-byte) hash.
Base64 | A group of similar binary-to-text encoding schemes that represent binary data in an ASCII string format by translating it into a radix-64 representation.

---

#### Table 1 : Glossary Table

## 2. SSM Middleware
This  document  describes  the  interface  standard  for  integrating  to  SSM  Middleware.  It  covers  the  transport protocol, web service standard and subscription requirement. As illustrstrated below, there are   few   security   configurations   and   settings   need   to   be implemented   to   ensure   secure   communication between servie requestor and service provider. 
##

#### ![](src/Figure 1.png)

##### 2.1 What needs to be done for connecting to SSM Middleware
|  |  | Example |
| ------------ | ------------- | ------------ |
| 1 | Service Requestor (i.e. Agency) need an account in Middleware System. <br>Please refer to [3.1](http://127.0.0.1:8000/markdownFile/GettingStarted/#31-agency-profile)| Liaosn with SSM Business Development team to have an account in the SSM Middleware. Login credential, username & password, will be sent to respective Service Requestor once the service requestor account is created.  | 
| 2 | Service Requestor is required to subscribe the services from the Service Catalog. <br> Please refer to 0  | Service Requestor login to system by using the login credential provided by the SSM. |
| 3 | Modifythe application for callingrequeirdservices. <br>Please refer to [4](http://127.0.0.1:8000/markdownFile/GettingStarted/#1-glosary) for username token implementation  | - Perform wsdl URL call to SSM Middleware to extract the webservice signature (WSDL). <br> - Develop soap message as per the SSM Middleware soap message standard. <br> - Inlcude HTTP Server username token as per SSM Middleware standard.  |
| 4|  Service Requestor application requires to connect SSM Middleware through HTTPS.  | HTTPS will be implemented in SSM Middleware. |

---

## 3. Subscription Process

#### ![](src/Figure 2.png)

* Each Service Requestor / Agency is required to register an account in SSM Middleware before it can connect to Middleware.
* Username and password will be sent to Service Requestor via email once the account is created.
* Service Requestor subscribes to the services by using the provided username and password. 
* The service subscription is required approval from SSM. Once the subscription is approved, Service Requestor is able to connect the SSM Middleware as long as the request message compliance to interface message format.

##### 3.1 Agency Profile

a. SSM MBDD need to create an account in Middleware for agency.
b. Once agency profile is created, a notification email will be sent to the agency.
c. Once agency profile is created, a notification email will be sent to the agency.