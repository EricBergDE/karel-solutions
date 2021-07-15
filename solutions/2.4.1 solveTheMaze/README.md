# 2.4.1 solveTheMaze

## Lösung

```java
void solveTheMaze()
{
    while (!onBeeper()) {
        if (frontIsClear()) {
            moveForward();
        } else if (leftIsClear()) {
            turnLeft();
        } else {
            turnRight();
        }
    }
    pickBeeper();
}
```
