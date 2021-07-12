# 2.4.3 addFast

## Lösung

```java
void addFast() {
    repeat (8) {
        if (onBeeper() && beeperAhead()) {
            moveForward();
            if (beeperAhead()){
                setSumAndCarryBit();
            } else {
                setCarryBit();
            }
        } else if (onBeeper() || beeperAhead()) {
            moveForward();
            if(beeperAhead()){
                setCarryBit();
            } else {
                setSumBit();
            }
        } else {
            moveForward();
            if (beeperAhead()) {
                setSumBit();
            } else {
                setNoBit();
            }
        }
        moveForward();
        moveForward();
        turnAround();
    }
}

void setNoBit() {
    moveForward();
    moveForward();
    turnRight();
    moveForward();
    turnRight();
    moveForward(); 
}

void setSumBit() {
    moveForward();
    moveForward();
    dropBeeper();
    turnRight();
    moveForward();
    turnRight();
    moveForward();
}

void setCarryBit() {
    moveForward();
    moveForward();
    turnRight();
    moveForward();
    turnRight();
    moveForward();
    dropBeeper();
}

void setSumAndCarryBit() {
    moveForward();
    moveForward();
    dropBeeper();
    turnRight();
    moveForward();
    turnRight();
    moveForward();
    dropBeeper();
}
```

(Lösung von @ron-png, leicht abgeändert)
