# 2.3.2 findTeddyBear

## Lösung

```java
void findTeddyBear()
{
    walkToEdge();
    while (!onBeeper()) {
        walkAlongEdge();
    }
    pickBeeper();
}

void walkToEdge()
{
    while (frontIsClear() && !onBeeper()) {
        moveForward();
    }
}

void walkAlongEdge()
{
    turnLeft();
    walkToEdge();
}

```
