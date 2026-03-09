  # robotArmV1
This project was about building an analogue servo controller for the AL5D robotic arm without using a microcontroller. We used 555 timers to generate PWM signals and directly control the arm’s joints. The goal was to get hands-on experience with circuit design, PWM generation, and open-loop control.

## What We Did

We used a dual-555 timer setup:

- **OHardware Assembly**: Set up the dual 555-timer circuit and connected it to the servo motors of the AL5D arm.
  
- **PWM Modulator**:Used one timer as an astable oscillator (50 Hz pulse) and the second as a monostable modulator to vary pulse width with a potentiometer.

- **Testing & Troubleshooting**:Measured signals with an oscilloscope and used a multimeter to check power stability and circuit connections.
  
- **Output**: These pulses drive the servos, moving the arm according to the signal width.

This is a simple open-loop control the circuit doesn’t check the arm’s actual position.


## What We Learned

- **Breadboard & Wiring**: Loose power rails or poor connections can cause the circuit to fail.

- **Component Quality**: A faulty potentiometer can stop the PWM signal; analogue systems rely heavily on component reliability.

- **Open-Loop Limitations**: Without feedback, the arm can’t compensate for extra weight or friction.


### Reflection
It was rewarding to see the arm respond directly to turning a knob. The project improved our skills in analogue circuit design, signal timing, and systematic troubleshooting. It also highlighted the challenges of open-loop control compared to microcontroller-based solutions.

## Future Improvements
- [ ] Add feedback sensors to implement closed-loop control.
- [ ] Integrate a microcontroller to allow programmable motion sequences.
