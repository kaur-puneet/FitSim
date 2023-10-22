# Fit-Sim Workout Simulator

Fit-Sim is a workout simulator that allows you to engage in virtual workouts or simply watch along as animations guide you through various exercises. The simulator provides four different workouts to choose from: push-ups, running, jump-roping, and planks.

## Technical Details

- **Platform:** Fit-Sim is designed to run on a DE1-SoC board. The FPGA allows for real-time control and interaction with various I/O devices.

- **I/O Devices:** Fit-Sim utilizes multiple input and output devices to provide an immersive experience:

  - **VGA:** The VGA output is used to display workout animations and user interfaces on a monitor or screen.

  - **HEX Display:** The HEX display shows real-time information during workouts, such as countdowns for push-ups and jump-rope exercises, and displays the user's total score at the end of each workout.

  - **Switches (SW):** Switches are used for user input, enabling users to configure workout parameters, such as the number of push-ups, workout duration, and speed settings.

  - **Keys (KEY):** Keys are used for navigation and workout selection. Users can start workouts and return to the workout selection page using these keys.

- **Code Implementation:** The Fit-Sim project is implemented in the C programming language. It includes functions for animating workouts, handling user input, and displaying information on the VGA and HEX display.

- **Scoring System:** Fit-Sim includes a scoring system that tracks the user's performance in workouts. Points are awarded for completing exercises, and the user's total score is displayed on the HEX display. A maximum score of 999 is allowed, and the score is reset upon reaching this limit.

 ## How It Works

1. **Workouts Selection:** On the starting page, users can press specific keys to access the workout selection page. These keys correspond to the four available workouts: push-ups (Key 0), running (Key 1), jump-rope (Key 2), and planks (Key 3).

2. **Workout Configuration:** Depending on the selected workout, users are prompted to input specific parameters. For instance, for push-ups, users specify the number of push-ups to complete, while for running, they set the duration and speed.

3. **Numerical Input:** Users use the switches (SW) to select numerical input. Key 0 is used for the first input, and Key 1 is used for the second input. For speed settings, a lower number corresponds to a higher speed.

4. **Workout Animation:** Fit-Sim provides real-time animation for each workout. For example, it shows a countdown of the remaining number of push-ups or jumps on the HEX display as the animation runs.

5. **Scoring:** After completing a workout, points are awarded, and the user's total score is displayed on the HEX display. If the maximum score of 999 is reached, the points are reset.

6. **Navigation:** Users can press any KEY to return to the workout selection page after completing a workout.


