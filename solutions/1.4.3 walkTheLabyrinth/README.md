# 1.4.3 walkTheLabyrinth

## Lösung

```java
void walkTheLabyrinth() {
    repeat (99) {
        if (!frontIsClear()) {
            if (leftIsClear()) {
                turnLeft();
            } else {
                turnRight();
            }
        }
        moveForward();
    }
}
```
