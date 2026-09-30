# amplifier-
# Amplifier Voltage Gain Calculator

Vin = float(input("Enter input voltage (V): "))
Vout = float(input("Enter output voltage (V): "))

if Vin != 0:
    gain = Vout / Vin
    gain_db = 20 * __import__('math').log10(abs(gain))

    print("Voltage Gain =", gain)
    print("Voltage Gain in dB =", gain_db, "dB")
else:
    print("Input voltage cannot be zero.")
