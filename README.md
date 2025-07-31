# 🛠️ Creating a New Project in STM32CubeIDE (Nucleo-G071RB)

## 📋 Prerequisites

- STM32CubeIDE installed.
- Nucleo-G071RB development board connected via USB.
- Basic knowledge of C and STM32 microcontrollers.

---

## 1. Create a New Project

1. Open **STM32CubeIDE**.
2. Go to `File > New > STM32 Project`.
3. In the **Board Selector** tab:
   - Type `Nucleo-G071RB` in the search bar.
   - Select the board and click **Next**.

---

## 2. Configure the Project

1. Enter a **project name** (e.g., `Blink_G071`).
2. Choose the project location.
3. Ensure the **Toolchain** is set to `STM32CubeIDE`.
4. Click **Finish**.

---

## 3. Configure Peripherals with STM32CubeMX

1. The **Device Configuration Tool** will open automatically.
2. In the pinout view:
   - Configure the pins you need (e.g., set `PA5` as GPIO Output for the onboard LED).
3. In the **Clock Configuration** tab, verify the system clock settings.
4. Save the `.ioc` configuration file.

---

## 4. Generate Code

1. Once the `.ioc`, there should be a pop up window to directly generate the code. Otherwise, click the gear icon or go to `Project > Generate Code`.
2. STM32CubeIDE will generate the base code using the HAL library.

---

## 5. Write Your Application Code

1. Open `Core/Src/main.c`.
2. Inside the `while (1)` loop, add your logic.
