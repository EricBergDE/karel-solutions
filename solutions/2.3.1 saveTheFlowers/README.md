# 2.3.1 saveTheFlowers

## Lösung

```java
void saveTheFlowers()
{
    repeat (5){
        climbOneUp();
        if (onBeeper()){
            pickBeeper();
        }
    }
    dropBeeper();
    repeat (3){
        climbOneDown();
        dropBeeper();
    }
    climbOneDown();    
}

void climbOneUp()
{
    turnLeft();
    while (!rightIsClear()){
        moveForward();
    }
    turnRight();
    moveForward();
}

void climbOneDown()
{
    moveForward();
    turnRight();
    while (frontIsClear()){
        moveForward();
    }
    turnLeft();
}
```
