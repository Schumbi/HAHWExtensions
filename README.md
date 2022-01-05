# HAHWExtensions

## Some hardware extensions for Home assistant
Repo containing my ESPHome yaml files with (perhaps) some advice.

### gaszaehler.yaml
Board: Wemos D1 Mini

This board counts ticks, that a reed relay produces. The gas meter has a rotating magnetised disc to calculate the gas volume. The mentions reed relay counts this ticks and adds them. For this task, the software uses the pulse_meter platform of ESPHome. The total value calculated is send to the home assistant instance. Furthermore, the software creates a number input, where the actual counter of the gas meter can be adjusted.
The board flashes it's blue onboard LED on every count.
