<a href="https://github.com/branilson"><img src="https://github.com/branilson/BL_TrafficLight/blob/master/img/180px-Traffic_lights_3_states.png" title="Branilson Luiz" alt="BranlsonLuiz"></a>

<!-- [![Branilson Luiz(https://github.com/branilson/BL_TrafficLight/blob/master/img/180px-Traffic_lights_3_states.png](https://github.com/branilson) -->


# Enhanced Traffic Light Mbed code

> Finite state machine code sample for a traffic light system with pedestrian call buttom, alert and off states.

> Made for ST STM32F4 Discovery board using ARM Mbed library and PlatformIO IoT Ecosystem.

> Challenge for students of the discipline Microprocessed Systems II at SENAI CIMATEC university center.

> Keywords: Traffic light, C/C++, PlatformIO, Mbed, STM32F4

**Finite State Machine policy**

- States: Red; Green; Yellow; Alert (Only Yellow blinking at 1Hz); Off.
- Initial state: Red
- Transition Red -> Green: t=10s
- Transition - Green --> Yellow: t=20s | buttom = 1
- Transition - Yellow --> Red: t=4s
- Transition - Any other state --> Alert: Buttom pressed t > 3s
- Transition - Any other state --> Off:  Buttom pressed 3s < t < 10s
- Transition - Off -- > Red:  Buttom pressed t > 10s
- Transition - Alert --> Previous state:  Buttom pressed 3s < t < 10s