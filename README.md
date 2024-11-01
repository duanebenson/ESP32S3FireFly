# ESP32S3FireFly
A Bluetooth network of digital "fireflies" powered by the Seeed Studio XIAO ESP32S3 boards

Sometimes even hobby projects go wrong.

The basis for this project isn’t complicated. I have a motion sensor and some capacitive sense inputs. Based on what those inputs say, I flash some LEDs in a pseudo random pattern. That’s the easy part.

I also though the Bluetooth LE mesh networking part would be easy. With BLE 5.0, mesh networks are supposed to be self-formable. In theory, I would form the network on wake up, transmit a signel to all network members waking them up using a wake-on-BT command, and then have each remote firefly flash a similar a pseudo random pattern in its LEDs.

However, apparently, BLE mesh isn’t yet supported with Arduino code in the XIAO ESP32S3 and C3 devices, as I’m using in this project.
I have a couple of links that might be helpful

ESPRESSIF: https://esp32.com/viewtopic.php?t=27814
Lucassvaz on Github: https://gist.github.com/lucasssvaz/bd105988aaf72ec291ecf94ecc2c692d

Mind you, they haven’t been helpful enough for me to get my project up and running, but may be someone else has been able to get BLE mesh running with Arduino code, and hopefully on an ESP32.

Check bask here periodically. I’d add to this as I get closer to a solution. And, if you have thoughts or places I can look, feel free to pass that on.
