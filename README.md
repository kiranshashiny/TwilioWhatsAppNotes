# TwilioWhatsAppNotes

Go to:

https://console.twilio.com/us1/develop/sms/overview

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/7608ee61-555e-4627-bb4e-1489148f6528)

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/eb38816a-26ea-4d2e-847b-f7d0f0816eb5)

Click on Send a WhatsApp Message

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/1278f177-3c3d-4968-89be-69e07cb68c6c)

Enter join selection-spell on your smartphone and you will get a message on your phone.

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/d8b85a46-4224-41de-a553-a17e7d04233e)



### Part 2


https://www.twilio.com/docs/usage/tutorials/how-to-set-up-your-php-development-environment

You will install the composer and all other things.

run the test.php

Run it as a web service.

Open the browser and see that you see the Helloworld message.

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/c9f94889-ee45-4fcb-aba7-92906b50d792)

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/d52c4b65-6260-497c-940e-23da00e426b2)


ngrok

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/ad3eb42f-7466-484b-ab17-3e94396d5634)


Go to the Ngrok referenced URL and it should say the Hello world message as well.


Next, https://www.twilio.com/blog/how-to-send-images-on-whatsapp-using-php


```
touch twilioWhatsAppMessaging.php .env
php composer.phar require twilio/sdk vlucas/phpdotenv
```

```
<?php

require_once "vendor/autoload.php";

use Twilio\Rest\Client;


$sid    = "PUT YOUR SID HERE";
$token  = "YOUR TOKEN HERE";

$twilio = new Client($sid, $token);

$message = $twilio->messages
                 ->create(
                     "whatsapp:+919845691854",
                     [
                              "mediaUrl" => ["https://images.unsplash.com/photo-1431250620804-78b175d2fada?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1600&h=900&fit=crop&ixid=eyJhcHBfaWQiOjF9"],
                              "from" => "whatsapp:+14155238886",
                              "body" => "Snacks maybe?"
                     ]
                 );
?>


```

![image](https://github.com/kiranshashiny/TwilioWhatsAppNotes/assets/14288989/7a79a38b-88c2-4cc6-a125-3d9207a5d2fd)




### Part 3:

Sending Images from Twilio WhatsApp using Node.js

https://www.twilio.com/blog/how-to-send-picture-whatsapp-using-twilio-and-javascript

![Uploading image.png…]()



Sending Images from Twilio WhatsApp using PHP

https://www.twilio.com/blog/how-to-send-images-on-whatsapp-using-php





