IR Remote Button Code Tester — WeMos D1 Mini + I²C LCD

Press any button on your remote and see its exact 32-bit hex code on a 16×2 LCD — even if the protocol shows as UNKNOWN.

What you'll learn:

How IR remotes send 38 kHz modulated signals

How the receiver demodulates and passes data to the board

Why UNKNOWN is normal (not an error)

How to handle 0xFFFFFFFF repeat frames

How to format codes as full 8-digit hex (0x%08X)

How to avoid LCD flicker with padded lines

Wiring:

IR OUT → D5 (GPIO14), VCC → 3.3V, GND → GND

LCD SDA → D2, SCL → D1, VCC → 5V, GND → GND

Libraries:

IRremoteESP8266

LiquidCrystal_I2C (Frank de Brabander)

Use it for: IR menus, relay control, LED triggers, motor/servo projects — compare the received code to a known value and act on it.

Key takeaway: UNKNOWN means the protocol is unnamed — the code is still valid and repeatable. Always use the first non-repeat hex value.

Code + wiring diagram in the description below.
