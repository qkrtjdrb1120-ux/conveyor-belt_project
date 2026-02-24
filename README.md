<img width="1071" height="520" alt="Screenshot from 2026-02-13 01-49-43" src="https://github.com/user-attachments/assets/03e4df12-17c4-48f3-a239-92fa80258cc5" />


system

PC
Web_Cam
[red, blue, yellow]
|
|
|--->STM32F411Re6 Board                                        STM32F411Re6 Board
|            |                                                       |    | ------> (STOP)data   : 0x1FF ------> conveyor_All_Stop_and_Roboat_IDLE
|            |--Tx                                              Rx --|    | ------> (Read)data   : 0x100 ------> conveyor_1         
|            |                                                       |    | ------> (Blue)data   : 0x101 ------> conveyor_2
|            |------- SPI                                  SPI ------|    | ------> (Yellow)data : 0x102 ------> conveyor_3
|            |------MCP2515-------------CAN-------------MCP2515------|    | ------> (Button)data : 0x103 ------> conveyor_4
|
|
|---> Basys3 Board
|           |           
|           |
|           |------------------------------>  SERVO_PWM_1  ----------->  MG996_SERVO_MOTOR_1
|           |------------------------------>  SERVO_PWM_2  ----------->  MG996_SERVO_MOTOR_2
|           |------------------------------>  SERVO_PWM_3  ----------->  MG996_SERVO_MOTOR_3
|           |------------------------------>  SERVO_PWM_4  ----------->  MG996_SERVO_MOTOR_4
|           |------------------------------>  SERVO_PWM_5  ----------->  MG996_SERVO_MOTOR_5
|           |------------------------------>  SERVO_PWM_6  ----------->  MG996_SERVO_MOTOR_6
|
|
