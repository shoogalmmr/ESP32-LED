# إضاءة لمبة LED متصلة بوحده ESP 
هذا مثال بسيط لإضاءة وإطفاء لمبة LED متصلة بوحدة ESP32 عند الطرف 18 (esp:18). يقوم هذا الكود بتشغيل وإطفاء اللمبة بشكل متكرر في حلقه loop. هذا يعني أن اللمبة ستكون مضاءة لمدة 100 ملي ثانية ثم مطفأة لمدة 100 ملي ثانية، وتستمر هذه الدورة إلى ما لا نهاية.

<img src= "https://github.com/user-attachments/assets/31094bef-b1d9-44dc-8bbe-1453726ad1e8" width="900" height="600">

## الكود

```
#define LEDPIN 18
void setup() {
  pinMode(LEDPIN , OUTPUT);
}

void loop() {

digitalWrite(LEDPIN, HIGH);
  delay(100); 
  digitalWrite(LEDPIN, LOW);
  delay(100);
}
``` 
