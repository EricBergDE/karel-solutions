# 1.1.2 defuseOneBomb

## Lösung

```java
void defuseOneBomb() {
    moveNineForward();
    pickBeeper();
    turnAround();
    moveNineForward();
    turnAround();
}

void moveNineForward() {
    repeat (9) {
        moveForward();
    }
}
```
