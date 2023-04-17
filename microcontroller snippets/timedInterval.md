# Timed Interval snippet

## header

```cpp
void timedInterval(const unsigned long& currentTime, const unsigned long& intervalMS, unsigned long& previousTime, void(*func)());
```

## cpp

```cpp
//cpp
void timedInterval(
  const unsigned long& currentTime,
  const unsigned long& intervalMS,
  unsigned long& previousTime,
  void(*func)()
) {
  if (currentTime - previousTime > intervalMS) {
    func();
    previousTime = currentTime;
  }
}
```

## example

```cpp
void loop() {
  timedInterval(lastTime, 12 * 1000, lastCall, [](){
    Serial.print("printing after 12 sec");
  });
}
```
