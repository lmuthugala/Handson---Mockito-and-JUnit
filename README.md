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
Consumer consumer = injector.getInstance(Consumer.class);
consumer.processMessages("Hi Lakith", "lakithmuthugala@gmail.com");
```
