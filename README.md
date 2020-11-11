# Handson---Mockito-and-JUnit

```java
public class MyApplication implements Consumer {

    Map<String, MessageService> serviceNameVSService;

    @Inject
    public  MyApplication (Set<MessageService> messageServices)
        //Read Set and initialize Map
    }

    @Override
    public void processMessages(String message, String receiver, String serviceType)
        //do some msg validation, manipulation logic etc
        MessageService messageService = serviceNameVSService.get(serviceType)
        messageService.sendMessage(message, receiver);
    }
}
```


```java
bind(MessageService.class).annotatedWith(Email.class).to(EmailService.class)
bind(MessageService.class).annotatedWith(SMS.class).to(SMSService.class)
```
