# pomodorod
Pomodoro daemon for use with your favorite status bar

## Installation

```
git clone https://github.com/terrifish/pomodorod.git
cd pomodorod/
chmod +x install.sh
./install.sh
```

## Usage

Starting the server:

```
pomodorod
```

Switching between "work" time and "break" time:

```
pomodoro toggle
```

Checking how much time is left:

```
pomodoro left
```

Resetting the timer:

```
pomodoro reset
```

Stopping the server:

```
pomodoro shutdown
```

Using with [polybar](https://github.com/jaagr/polybar):

```
[module/pomodoro]
type = custom/script
exec = pomodoro left
interval = 1
click-left = pomodoro toggle
click-right = pomodoro reset
format-prefix = " "
```
