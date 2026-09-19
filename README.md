int soil = A0;

void setup() {
  Serial.begin(9600);
}

void loop() {
  int value = analogRead(soil);

  Serial.print("Soil: ");
  Serial.println(value);

  if (value < 400)
    Serial.println("Dry Soil");
  else
    Serial.println("Wet Soil");

  delay(1000);
}
# Soil-Moisture-Monitor
