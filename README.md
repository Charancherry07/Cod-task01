# Cod-task01#include <LiquidCrystal.h>

// Initialize LCD display
LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

int count = 0;

void setup() {
  lcd.begin(16, 2);
  lcd.setCursor(0, 0);
  lcd.print("Counter:");
}

void loop() {
  lcd.setCursor(0, 1);
  lcd.print("Count: ");
  lcd.print(count);
  count++;
  delay(1000); // increment count every 1 second
}

