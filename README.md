<a href="https://github.com/branilson"><img src="https://github.com/branilson/BL_TrafficLight2/raw/master/img/trafficlight2.png" title="Branilson Luiz" alt="BranlsonLuiz"></a>

<!-- [![Branilson Luiz(https://github.com/branilson/BL_TrafficLight2/raw/master/img/trafficlight2.png](https://github.com/branilson) -->


# Enhanced Traffic Light Mbed code

> Finite state machine code sample for a traffic light system with pedestrian call buttom, alert and off states.

> Made for ST STM32F4 Discovery board using ARM Mbed library and PlatformIO IoT Ecosystem.

> Challenge for students of the discipline Microprocessed Systems II at SENAI CIMATEC university center.

> Keywords: Traffic light, Finite State Machine, C/C++, Mbed, STM32F4

**Finite State Machine policy**

- States: Red; Green; Yellow; Alert (Only Yellow blinking at 1Hz); Off.
- Initial state: Red
- Transition Red -> Green: t=10s
- Transition - Green --> Yellow: t=20s || tBt=<3s
- Transition - Yellow --> Red: t=4s
- Transition - Any other state --> Alert: tBt>=3s && tBt<10s
- Transition - Any other state --> Off: tBt>10s
- Transition - Off -- > Red: tBt > 10s
- Transition - Alert --> Previous state: tBt>=3s && tBt<10s
- t = elapsed time; tBt =  time Button pressed.

<a href="https://github.com/branilson"><img src="https://github.com/branilson/BL_TrafficLight2/raw/master/img/tl2_fsm.png" title="Branilson Luiz" alt="BranlsonLuiz"></a>