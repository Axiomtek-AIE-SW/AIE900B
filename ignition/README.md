# Smart Ignition Management
To access the Smart Ignition Management main menu, please enter the following command in the terminal:  
`$ psu2_axiomtek.sh`

Brief information about the current settings will be displayed at the bottom of the main menu:
 - **FW Version:** Current firmware version
 - **Ignition Management:** Enabled or Disabled
 - **Auto Power On:** Enabled or Disabled
 - **Vin Voltage:** Current Vin Voltage
 - **IGN Signal:** Current Ignition Signal (On or OFF)  
![image](https://github.com/user-attachments/assets/8dd6600b-ee7c-4442-b0e5-a0ea71e81006)

The Smart Ignition Management menu enables users to configure settings related to the vehicle ignition switch. The relevant ignition status setting values are displayed below:  
## a. The current setting
To view the detailed threshold settings of Smart Ignition, including the following items:
- Power-on Voltage (System powers on when voltage reaches this level)
- Undervoltage (System shuts down if voltage drops below this level)
- Undervoltage shutdown delay timer (if low voltage continues for the period)
- Ignition power-on delay timer (a delay when the ignition signal is detected)
- Ignition shutdown delay timer (a delay when the ignition signal is lost)

## b.	Ignition Management
- To enable or disable the function of Smart Ignition Management.
- To return to the main menu, select **"Cancel"**.

## c.	Advanced Settings
### 1)	Auto Power On Mode
To enable or disable Auto Power On Mode

### 2)	Power-On/Undervoltage Detection  
#### 2-1)	Power-On and undervoltage voltage threshold configuration  
To adjust the voltage value of undervoltage voltage threshold value (Range from 9.0 to 23.0V) and power-on voltage threshold value (Range from 9.0 to 24.0V)  
#### 2-2)	Undervoltage shutdown delay timer  
To adjust the undervoltage shutdown delay EndTime value (Range from 60 to 10800 seconds)  

### 3)	Ignition Power Delay  
#### 3-1)   Power-On Delay Timer  
To adjust Power-On delay EndTime value (Range from 2 to 1800 seconds)  
#### 3-2)	Shutdown Delay Timer:  
To adjust shutdown delay EndTime value (Range from 1 to 21600 seconds)  

### 4)	Cancel
To return to the main menu, select **"Cancel"**.  

## d.	Save Setting (Saves changes as the custom default)
To immediately save changes as the custom default, select **"d"** from the main menu. **“Save Settings …[OK]”** will be displayed once the saving process is complete.

## e.	Restore Default Setting
- To restore custom default or factory default from the EEPROM. **“Restore Custom Default …[OK]”** or **“Restore Factory Default…[OK]”** will be displayed once the restoration process is complete.
- To return to the main menu, select **"Cancel”**.

## x.	Exit
To exit the Smart Ignition Management main menu, select **“x”**.  

# View detailed current settings of Smart Ignition
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“a”** and press **“Enter”** to confirm. The detailed current settings of Smart Ignition will be displayed, and the system will automatically return to the main menu afterward.  
![image](https://github.com/user-attachments/assets/9b8f3983-5bcd-462b-851c-73870781ad14)

# Switch of the Smart Ignition Function
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“b”** and press **“Enter”** to confirm.  
**Step 3.**
- **To enable Smart Ignition Management:**  
Select **“1”** and the system will automatically return to the main menu afterward.
- **To disable Smart Ignition Management:**  
Select **“2”** and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/035542c6-0db8-4587-814b-74dc25201557)

# Auto Power On Mode Setting
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“c”** and press **“Enter”** to confirm.  
**Step 3.** Select **“1”** to open the Auto Power On Mode menu.  
**Step 4.**
- **To enable Auto Power On Mode:**  
Select **“1”** and the system will automatically return to the main menu afterward.
- **To disable Auto Power On Mode:**  
Select **“2”** and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/e650446e-5e18-4999-bd15-d7f16baf8471)

# Power-On/Undervoltage Detection Settings
**Step 1.** Access the Smart Ignition Management main menu.  
**Step 2.** Select **“c”** and press **“Enter”** to confirm.  
**Step 3.** Select **“2”** to open the Power-On/Undervoltage Detection menu.  
**Step 4.**  
- **To configure power-on and undervoltage voltage thresholds:**  
Select **“1”** then follow the on-screen instructions to enter the desired values, and the system will automatically return to the main menu afterward.
- **To exit without making changes:**  
Select **“3”** to return directly to the main menu.  
![image](https://github.com/user-attachments/assets/ffa83da2-da17-4f85-84a7-543abef0c365)

