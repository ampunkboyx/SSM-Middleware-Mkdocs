# Getting Started

# 1. Glosary
The following specify terms and abbreviations used in this document and their definitions that are needed to understand this document.
#

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

# 2. SSM Middleware
This  document  describes  the  interface  standard  for  integrating  to  SSM  Middleware.  It  covers  the  transport protocol, web service standard and subscription requirement. As illustrstrated below, there are   few   security   configurations   and   settings   need   to   be implemented   to   ensure   secure   communication between servie requestor and service provider. 
#

#### ![](src/Figure 1.png)

## 2.1 What needs to be done for connecting to SSM Middleware
|  |  | Example |
| ------------ | ------------- | ------------ |
| 1 | Service Requestor (i.e. Agency) need an account in Middleware System. <br>Please refer to [3.1](http://127.0.0.1:8000/markdownFile/GettingStarted/#31-agency-profile)| Liaosn with SSM Business Development team to have an account in the SSM Middleware. Login credential, username & password, will be sent to respective Service Requestor once the service requestor account is created.  | 
| 2 | Service Requestor is required to subscribe the services from the Service Catalog. <br> Please refer to 0  | Service Requestor login to system by using the login credential provided by the SSM. |
| 3 | Modifythe application for callingrequeirdservices. <br>Please refer to [4](http://127.0.0.1:8000/markdownFile/GettingStarted/#1-glosary) for username token implementation  | - Perform wsdl URL call to SSM Middleware to extract the webservice signature (WSDL). <br> - Develop soap message as per the SSM Middleware soap message standard. <br> - Inlcude HTTP Server username token as per SSM Middleware standard.  |
| 4|  Service Requestor application requires to connect SSM Middleware through HTTPS.  | HTTPS will be implemented in SSM Middleware. |

---
# 3. Subscription Process

#### ![](src/Figure 2.png)

* Each Service Requestor / Agency is required to register an account in SSM Middleware before it can connect to Middleware.
* Username and password will be sent to Service Requestor via email once the account is created.
* Service Requestor subscribes to the services by using the provided username and password. 
* The service subscription is required approval from SSM. Once the subscription is approved, Service Requestor is able to connect the SSM Middleware as long as the request message compliance to interface message format.

## 3.1 Agency Profile

a. SSM MBDD need to create an account in Middleware for agency.<br>
b. Once agency profile is created, a notification email will be sent to the agency.<br>
c. Email content include the admin user details.<br>
#### ![](src/UserID.png)
d. After that, you can use username and password to login the system.
#### ![](src/login.png)
e. Once login success will go to landing page.
#### ![](src/landingPage.png)

## 3.2 Service Catalog – Service Subscription

a. Login into the  system
#### ![](src/login.png)

b. Select the Subscription screen
#### ![](src/SubscriptionScreen.png)

c. Subscription New Service
#### ![](src/SubscriptionSservice.png)

d. Select the service category to subscribe
#### ![](src/ServiceCatalog.png)

e. Once confirm click on the “save” button

#### ![](src/ConfirmationPage.png)

f. After click subscribe button will pending SSM approval to approve it.<br>
g. Receive email when the service category approved.<br>
#### ![](src/ApprovedEmail.png)

## 3.3 ENDPOINT URL
You can view the endpoint URLs for your subscribed service catalogs in the integrasi portal. They look similar to the samples below.
#
Production URL:<br>
https://integrasi.ssm.com.my/{Service Catalog Name}/{version no}
#
Testing URL:<br>
https://integrasi.ssm.com.my/testing/{Service Catalog Name}/{version no}
#
Example:<br>
https://integrasi.ssm.com.my/BusinessService/1

## 3.4 Message Format

Sample Request Message<br>
```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
    <soapenv:Header/>
    <soapenv:Body>
        <rob:FindBusinessByBrNo xmlns:rob="urn:ssm/rob">
            <header>
            </header>
                <customerId>AGENCY</customerId>
                <customerReferenceNo>1234</customerReferenceNo>
                <customerTransactionDate>2016-08-09T16:00:00.000Z</customerTransactionDate>
            <request>
                <brNo>001234567</brNo>
                <agencyBranchCode>KL</agencyBranchCode>
            </request>
        </rob:FindBusinessByBrNo>
    </soapEnv:Body>
</soapEnv:Envelope>
```
#
Good Response Message
```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
    <soapenv:Header/>
    <soapenv:Body>
        <rob:FindBusinesByBrNoResponse xmlns:rob="urn:ssm/rob">
            <header>
                <customerId>AGENCY</customerId>
                <customerReferenceNo>1234</customerReferenceNo>
                <customerTransactionDate>2016-08-09T16:00:00.000Z</customerTransactionDate>
                <serviceCode>CBS00002</serviceCode>
                <versionNumber>1</versionNumber>
                <errorCode/>
                <errorMessage/>
                <recordCount>1</recordCount>
                <requestTimestamp>2016-08-09T16:00:00.123Z</requestTimestamp>
                <responseTimestamp>2016-08-09T16:00:00.567Z</responseTimestamp>
                <hostReferenceNo/>
                <hostStatusCode/>
                <hostStatusMessage/>
            </header>
            <request>
                <brNo>001234567</brNo>
                <agencyBranchCode>KL</agencyBranchCode>
            </request>
            <response>
                <businessInfoList>
                    <businessInfo>
                        <businessName>...</businessName>
                        ...
                    </businessInfo>
            </response>
        </rob:FindBusinessByBrNoResponse>
    </soapenv:Body>
</soapenv:Envelope>
```
#
Error Response Message
```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"><soapenv:Header/>
    <soapenv:Body>
        <rob:FindBusinesByBrNoResponse xmlns:rob="urn:ssm/rob">
            <header>
                <customerId>AGENCY</customerId>
                <customerReferenceNo>1234</customerReferenceNo>
                <customerTransactionDate>2016-08-09T16:00:00.000Z</customerTransactionDate>
                <serviceCode>CBS00002</serviceCode>
                <versionNumber>1</versionNumber>
                <errorCode>ESB00002</errorCode>
                <errorMessage>Host Time-out</errorMessage>
                <recordCount>0</recordCount>
                <requestTimestamp>2016-08-09T16:00:00.123Z</requestTimestamp>
                <responseTimestamp>2016-08-09T16:00:35.567Z</responseTimestamp>
                <esbHost>mwmbp01.ssm.com.my</esbHost>
                <hostReferenceNo/>
                <hostStatusCode/>
                <hostStatusMessage/>
            </header>
            <request>
                <brNo>001234567</brNo>
                <agencyBranchCode>KL</agencyBranchCode>
            </request>
        </rob:FindBusinessByBrNoResponse>
    </soapenv:Body>
</soapenv:Envelope>
```