# I/O Power Management

## USB_VBUS_Power0 (CN3)
- The default USB_VBUS_Power0 state is ON
- Reset Power 
```
gpioset --mode=time --sec=1 `gpiofind "PY.04"`=0
```
- Power off
```
gpioset --mode=signal `gpiofind "PY.04"`=0 &
PID=$!
```
- Power on
```
sudo kill $PID
```

## USB_VBUS_Power1 (CN4)
- The default USB_VBUS_Power1 state is ON
- Reset Power 
```
gpioset --mode=time --sec=1 `gpiofind "PZ.01"`=0
```
- Power off
```
gpioset --mode=signal `gpiofind "PZ.01"`=0 &
PID=$!
```
- Power on
```
sudo kill $PID
```

## POE_Power
- The default POE_power state is ON
- Reset Power 
```
gpioset --mode=time --sec=1 `gpiofind "PCC.01"`=0
```
- Power off
```
gpioset --mode=signal `gpiofind "PCC.01"`=0 &
PID=$!
```
- Power on
```
sudo kill $PID
```

## B-Key_Power
- The default B-Key_Power state is ON
- Reset Power 
```
gpioset --mode=time --sec=1 `gpiofind "PAC.06"`=0
```
- Power off
```
gpioset --mode=signal `gpiofind "PAC.06"`=0 &
PID=$!
```
- Power on
```
sudo kill $PID
```

## mini-PCIe_Power
- The default mini-PCIe_Power state is ON
- Reset Power 
```
gpioset --mode=time --sec=1 `gpiofind "PEE.02"`=0
```
- Power off
```
gpioset --mode=signal `gpiofind "PEE.02"`=0 &
PID=$!
```
- Power on
```
sudo kill $PID
```

## CAN1 Termination Resistor
- The default CAN1_TR is disable
- CAN1_TR Enable
```
gpioset --mode=signal `gpiofind "PCC.03"`=0 &
PID=$!
```
- CAN1_TR disable
```
sudo kill $PID
```

## CAN2 Termination Resistor
- The default CAN2_TR is disable
- CAN2_TR enable
```
gpioset --mode=signal `gpiofind "PQ.06"`=0 &
PID=$!
```
- CAN2_TR disable
```
sudo kill $PID
```
