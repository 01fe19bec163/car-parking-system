# car-parking-system
A simple car parking system is implemented wherein whenever the entrance sensor is triggered, the passwrod is requested and if the passsword is correct the gate opens otherwise remains closed. There is also a need to take care of a scenario where if the car entering gets detected by the exit sensor and at the same time another car comes, the gate should close and request password for the comming car.
The system is implemented using FSM with states as: idle, wait_password, right_password, wrong_password, stop.
From right_password state if both entrance and exit sensor get triggered then next state will be stop state and remains in this state until password entered is correct.
From right_password state if exit sensor is triggered then next state will be idle state.
