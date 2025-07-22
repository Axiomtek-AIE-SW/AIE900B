
# Default Setting

**DIO1 ~ DIO8 are set to INPUT by default.**

> **Note:**  
> The DIO protocol will reset to the default setting after a cold boot.

---

# 1. Command Format

```bash
i2cset -f -y <i2c_num> <device_addr> <reg_addr> <value>
i2cget -f -y <i2c_num> <device_addr> <reg_addr>
```

**Example:**

- `<i2c_num>`: `7`
- `<device_addr>`: `0x24` or `0x25`
- `<reg_addr>`: `0x00` or `0x01` or `0x03`
- `<value>`:
  - Bit0 → DIO1, Low: `0`, High: `1`
  - Bit1 → DIO2, Low: `0`, High: `1`
  - ...
  - Bit7 → DIO8, Low: `0`, High: `1`

---

# 2. DIO Output Sample Code

```bash
# Set DIO1 ~ 8 as Output
i2cset -f -y 7 0x24 0x03 0x00

# Set DIO1 ~ 8 as High
i2cset -f -y 7 0x24 0x01 0xFF

# Set DIO1 ~ 4 as Low and DIO5~8 as High
i2cset -f -y 7 0x24 0x01 0xF0

# Set DIO1 as High and DIO2~8 as Low
i2cset -f -y 7 0x24 0x01 0x01

# Set DIO1 ~ 4 as Input and DIO5~8 as Output
i2cset -f -y 7 0x24 0x03 0x0F
```

---

# 3. DIO Input Sample Code

```bash
# Set DIO1 ~ 8 as Input
i2cset -f -y 7 0x24 0x03 0xFF
   
# Read all inputs
i2cget -f -y 7 0x24 0x00
```
