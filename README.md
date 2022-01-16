# Dramcontroller
HID controller board design for Engineering Experience 2
Below the periferals with corresponding pins are described. 
A distinction between the on-board periferals, I2C addresses and sensor slots makes this pin overview clear. 

## On board periferals
| Periferal | Corresponding GPIO Pin  |
|---|---|
| Buzzer | 2 |
| Vibrator 1 | 12 |
| Vibrator 2 | 5 |
| Debug LED | 13 |
| IO Expender INT | 11 |

## I2C addresses
Four IO expanders connected with the I2C bus control the 7 segment displays, led indicator array and GPIO 3 from every sensor slot. I2C sensors should use always other addresses to prevent collisions during operation.

| IO Expander | Corresponding I2C addres  |
|---|---|
| Segment display 1 | 0x38 |
| Segment display 2 | 0x39 |
| Led array | 0x3A |
| Sensor slot GPIO 3 | 0x3B |


## Sensor slots
### Sensor slot 1
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 6 | Digital |
| GPIO 2 | 14  | Digital - Analog |
| GPIO 3 | IO EXP pin 1 | Digital (0b00000001) |
| UART  |  | Serial |
| I2C  |  |  |

### Sensor slot 2
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 39 | Digital |
| GPIO 2 | 15  | Digital - Analog |
| GPIO 3 | IO EXP pin 2 | Digital (0b00000010) |
| UART  |  | Serial |
| I2C  |  |  |

### Sensor slot 3
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 8 | Digital |
| GPIO 2 | 16  | Digital - Analog |
| GPIO 3 | IO EXP pin 3 | Digital (0b00000100) |
| UART  |  | Serial |
| I2C  |  |  |

### Sensor slot 4
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 9 | Digital |
| GPIO 2 | 17  | Digital - Analog |
| GPIO 3 | IO EXP pin 4 | Digital (0b00001000) |
| UART  |  | Serial |
| I2C  |  |  |

### Sensor slot 5
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 10 | Digital |
| GPIO 2 | 18  | Digital - Analog |
| GPIO 3 | IO EXP pin 5 | Digital (0b00010000) |
| UART  |  | Serial1 |
| I2C  |  |  |

### Sensor slot 6
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 23 | Digital |
| GPIO 2 | 19  | Digital - Analog |
| GPIO 3 | IO EXP pin 6 | Digital (0b00100000) |
| UART  |  | Serial1 |
| I2C  |  |  |

### Sensor slot 7
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 24 | Digital |
| GPIO 2 | 4  | Digital - Analog |
| GPIO 3 | IO EXP pin 7 | Digital (0b01000000) |
| UART  |  | Serial1 |
| I2C  |  |  |

### Sensor slot 8
| Periferal | Pin | Comment |
|---|---|---|
| GPIO 1 | 22 | Digital |
| GPIO 2 | 3  | Digital - Analog |
| GPIO 3 | IO EXP pin 8 | Digital (0b10000000) |
| UART  |  | Serial1 |
| I2C  |  |  |

