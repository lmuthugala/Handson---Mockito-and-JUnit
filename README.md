# Handson---Mockito-and-JUnit

```java
public class MyApplication implements Consumer {

    private MessageService messageService;

    @Inject
    public  MyApplication (MessageService messageService) {
        this.messageService = messageService;
    }

    @Override
    public void processMessages(String message, String receiver) {
        //do some msg validation, manipulation logic etc
        this.messageService.sendMessage(message, receiver);
    }
}
```


```java
@Qualifier
@Target({ FIELD, PARAMETER, METHOD })
@Retention(RUNTIME)
public @interface AuthToken {
}
```
