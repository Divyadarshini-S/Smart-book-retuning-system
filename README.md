from time import sleep
import twilio
import twilio.rest
from twilio.rest import Client
from datetime import datetime

now = datetime.now()
dt_string = now.strftime("%d/%m/%Y %H:%M:%S")

account_sid = "AC450016f09d39e5d2e915db3b40cbca7a"  

auth_token = "fd9517abdfe5e06f9c85399b1c1b5ac8"
client = Client(account_sid, auth_token)
 
while 1:
    print'show u product...'
    scode = raw_input(" ")
    #print(scode)
    u=scode[0:5]
    
    #print u
    if(u=="26081"):
        print 'FPGA Based System Design'
        message = client.api.account.messages.create(to="+919944204570", from_="+14178922779",
                                        body="VCEW,date and time :"+dt_string+"Book:"+u+"Recieved")
        print ("msg Sending...")
        sleep(3)
       
    if(u=="29980"):
        print 'Python Programming'
        message = client.api.account.messages.create(to="+919944204570", from_="+14178922779",
                                        body="VCEW,date and time :"+dt_string+"Book:"+u+"Recieved")
        print ("msg Sending...")
        sleep(3)
        
    if(u=="30378"):
        print 'JAVA'
        message = client.api.account.messages.create(to="+919944204570", from_="+14178922779",
                                        body="VCEW,date and time :"+dt_string+"Book:"+u+"Recieved")
        print ("msg Sending...")
        sleep(3)
       
    if(u=="29187"):
        print 'Digital Design'
        message = client.api.account.messages.create(to="+919944204570", from_="+14178922779",
                                        body="VCEW,date and time :"+dt_string+"Book:"+u+"Recieved")
        print ("msg Sending...")
        sleep(3)
