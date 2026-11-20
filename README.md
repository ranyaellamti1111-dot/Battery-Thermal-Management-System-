# Battery Thermal Management System

A team engineering project comparing passive and fan-assisted cooling for an automotive lithium-ion battery module. We used MATLAB and Simulink to study the thermal response and developed an Arduino-based controller for temperature monitoring and PWM fan control.

## Physical prototype

![Physical BTMS prototype with its enclosure, Arduino board, wiring, and cooling fan](prototype.png)

## Simulink models

### Passive cooling baseline

The baseline models the module's thermal response with the fans off.

![Simulink model for passive battery cooling](simulink-passive.png)

### Fan-assisted cooling

The second model adds active airflow so we can compare the temperature response with the passive case.

![Simulink model for fan-assisted battery cooling](simulink-active.png)

## Simulation results

Under the simulated conditions shown in the project presentation, fan-assisted cooling held the temperature around **40 °C**, while the passive case exceeded the project's **45 °C design target**.

![Simulated temperature comparison for active and passive cooling](temperature-comparison.png)

## Arduino monitoring and control

The controller monitors temperature and uses PWM to drive the cooling fans. The project also included alert and current-limiting logic for elevated temperatures.

[View the Arduino wiring diagram](docs/images/arduino-wiring.png)
