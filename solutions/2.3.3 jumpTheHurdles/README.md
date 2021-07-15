# 2.3.3 jumpTheHurdles

## Lösung

```java
void jumpTheHurdles()
{
    turnLeft();
    while (!onBeeper()) {  
        while (!rightIsClear()) {
            moveForward();
        }
        turnRight();
        moveForward();
        turnRight();
        while (frontIsClear()) {
            moveForward();
        }
        turnAround();
    }
    pickBeeper();
}
```
