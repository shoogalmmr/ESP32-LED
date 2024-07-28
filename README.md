# إضاء لمبة LED متصلة بوحده ESP 
هذا مثال بسيط لإضاءة وإطفاء لمبة LED متصلة بوحدة ESP32 عند الطرف 18 (esp:18). يقوم هذا الكود بتشغيل وإطفاء اللمبة بشكل متكرر في حلقه loop. هذا يعني أن اللمبة ستكون مضاءة لمدة 100 ملي ثانية ثم مطفأة لمدة 100 ملي ثانية، وتستمر هذه الدورة إلى ما لا نهاية.
##الكود
'''
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
'''
 
