# 1.4.2 removeTheTiles

Auf jedem Feld liegt ein Beeper, die Karel von außen nach innen aufheben muss.

## Lösung

```java
void removeTheTiles() {
    repeat (100) {
        pickBeeper();
        if (!frontIsClear() || !beeperAhead()) {
            turnLeft();
        }
        moveForward();
    }
}
```

## Erklärung

Siehe auch [tileTheFloor](../1.3.4%20tileTheFloor).
