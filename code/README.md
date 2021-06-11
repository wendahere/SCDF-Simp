
## Hi this is where the codes are 
##### 1.0 install esp 
run arduino ide and make sure all the libary are 
installed approprietly 
##### following libary are required
- pubsubclient
- esp 32 
- dht 11(current code uses dht 11 to simulate obd port data)


###### Things to change in code
```sh
const char* ssid = "put password here";
const char* password = "put password";
#define DHTPIN 4 
#define DHTTYPE DHT11
#define ORG "insert org" 
#define DEVICE_TYPE "inside type" 
#define DEVICE_ID "inert id" 
#define TOKEN "insert code"  
```
## how to set up ibm watson iot 
##### here's a small guide
-set up ibm cloud account 
-look for watson iot and create 
-set up device as shown below 
![Test Image 5](https://github.com/wendahere/SCDF-Simp/blob/main/code/pictures/registerdevice.PNG?raw=true)
-take note of credentials (to be pasted above in ino code)
![Test Image 5](https://github.com/wendahere/SCDF-Simp/blob/main/code/pictures/registerdevice.PNG?raw=true)


### testing ibm iot 
- go to boards and create a line chart if everything goes well you should be seeing data being 
![Test Image 5](https://github.com/wendahere/SCDF-Simp/blob/main/code/pictures/dashboard.PNG.jpg?raw=true)

## Troubleshooting watson iot
-change the sercurity option to tls optional 
![Test Image 5](https://github.com/wendahere/SCDF-Simp/blob/main/code/pictures/tls.jpg?raw=true)


### 2.0 node red 
- go to ibm cloud and install node red starter
- make sure to not give instance memory  more then 256 as lite account max limit is 256 mb 

















