# The robot serial does not connect to ttyACM0

Some robots might use the Arduino clone board called "Geekcreit". If that is the case (you can check by looking at the board), call `connect()` with `ttyUSB0` instead.

# I can't connect the raspberry pi to the internet

Due to reasons, the system clock needs to be up to date to be able to access the internet.

Set the date using the `date` program in bash

```bash
date --set="23 August 2024 12:55:00"
```

# A command I am trying to run says the operation is not permitted

Use `sudo` to elevate your priviledge. Example:

```bash
sudo date --set="23 August 2024 12:55:00"
```

You need to provide your user password.