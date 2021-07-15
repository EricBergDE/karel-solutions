# 2.2.3 addSlow

## Lösung

```java
void addSlow()
{
    while (frontIsClear() || rightIsClear()) {
        decrement();
        changeToSecond();
        increment();
        changeToFirst();
    }
}

void changeToSecond()
{
    turnAround();
    while (frontIsClear()) {
        moveForward();
    }
    turnRight();
    moveForward();
    turnRight();
}

void changeToFirst()
{
    turnAround();
    while (frontIsClear()) {
        moveForward();
    }
    turnLeft();
    moveForward();
    turnLeft();
}

void decrement()
{
    while (! onBeeper()) {
        dropBeeper();
        moveForward();
    }
    pickBeeper();
}

void increment()
{
    while (onBeeper()) {
        pickBeeper();
        moveForward();
    }
    dropBeeper();
}
```
