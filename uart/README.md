# UART
- Supports RS-232, RS-422, and RS-485

## Read UART Mode
```
cat /sys/devices/platform/f81435_mode_ctrl/f81435/uartMode
```

## Set UART Mode
```
# Set RS-232
echo rs232 > /sys/devices/platform/f81435_mode_ctrl/f81435/uartMode

# Set RS-422
$ echo rs422 > /sys/devices/platform/f81435_mode_ctrl/f81435/uartMode

# Set RS-485
$ echo rs485 > /sys/devices/platform/f81435_mode_ctrl/f81435/uartMode
```
