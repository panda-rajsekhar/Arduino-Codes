# LED Blinker_400ms
This project deals with the blinking of 3 leds Red Green and Yellow using an Arduino Uno R3 embedded development board , some jumper cables , a breadboard  and 3 220 ohm resistors 

## Step 1
First of all we need to understand how to blink one led with  the help of 13th GPIO pin 

### **Components Needed:**

- **Arduino Uno Rev3**
- **Breadboard**
- **LED** (preferably red for testing)
- **Resistor** (220Ω or 330Ω recommended)
- **Jumper Wires**

---

### **Circuit Setup:**

1. **Connect the LED to the Breadboard**
    
    - Place the LED on the breadboard.
    - The longer leg is the **anode** (positive) and should be connected to the digital pin via a resistor.
    - The shorter leg is the **cathode** (negative) and should connect to the **GND** pin.
2. **Add the Resistor**
    
    - Connect one end of the resistor to the anode of the LED.
    - The other end of the resistor will connect to one of the Arduino’s **digital pins** (e.g., Pin 13).
3. **Wire the Cathode to Ground**
    
    - Use a jumper wire to connect the cathode of the LED to the Arduino’s **GND** pin.
4. **Power the Arduino**
    
    - Connect your Arduino Uno to your computer using a USB cable.

---

### **Code to Blink the LED**

```cpp
// Pin assignment
int ledPin = 13; // LED connected to digital pin 13

void setup() {
  pinMode(ledPin, OUTPUT); // Set pin 13 as an output
}

void loop() {
  digitalWrite(ledPin, HIGH); // Turn the LED on
  delay(1000);               // Wait for 1 second
  digitalWrite(ledPin, LOW);  // Turn the LED off
  delay(1000);               // Wait for 1 second
}
```

---

### **Steps to Upload Code:**

1. Open the Arduino IDE on your computer.
2. Select the correct **Board** and **Port** from the **Tools** menu.
    - Board: **Arduino Uno**
    - Port: Check the COM port the Arduino is connected to.
3. Copy and paste the code above into the IDE.
4. Click the **Upload** button (arrow pointing right).



* After being able to blink a single led with Arduino we will move forward to blink 3 LED's with the pin 13, 12, 11 of the Arduino Board and we will be making the connections as per the schematic given or the circuit diagram uploaded.

* The circuit is simulated using Tinker Cad 
Tinkercad is a free web app for 3D design, electronics, and coding. We’re the ideal introduction to Autodesk, a global leader in design and make technology. 

