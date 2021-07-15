# 1.3.3 cleanTheRoom

## Lösung von [@EricBergDE](https://github.com/EricBergDE)

```java
void cleanTheRoom()
{
    repeat (5){ 
        cleanALine();
        leftTurn();
        cleanALine();
        if (rightIsClear()){
            rightTurn();
        }
    }
}

void cleanALine()
{
    repeat (10){
        if (onBeeper()){
            pickBeeper();
            if (frontIsClear()){
                moveForward();
            }
        } else {
            if (frontIsClear()){
                moveForward();
            }
        }
    }
}
```
