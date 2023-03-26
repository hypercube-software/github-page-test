# Headline

> An awesome project.

![build](https://github.com/hypercube-software/github-page-test/workflows/Node.js%20CI/badge.svg)

## Latex

Inline mode: $J(\theta )= \frac{1}{2m}\left( {{\theta }^{T}}{{X}^{T}}X\theta -{{\theta}^{T}}{{X}^{T}}y-{{y}^{T}}X\theta + {{y}^{T}}y \right) $ equation.

Inline mode: $J(\theta) = - \frac{1}{m} \sum_{i=1}^m [ y^{(i)}\ \log (h_\theta (x^{(i)})) + (1 - y^{(i)})\ \log (1 - h_\theta(x^{(i)}))] + \frac{\lambda}{2m}\sum_{j=1}^n \theta_j^2$ equation 2.

Display mode:
$$
J(\theta) = - \frac{1}{m} \sum_{i=1}^m [ y^{(i)}\ \log (h_\theta (x^{(i)})) + (1 - y^{(i)})\ \log (1 - h_\theta(x^{(i)}))] + \frac{\lambda}{2m}\sum_{j=1}^n \theta_j^2
$$


Display mode with tag:
$$
J(\theta) = - \frac{1}{m} \sum_{i=1}^m [ y^{(i)}\ \log (h_\theta (x^{(i)})) + (1 - y^{(i)})\ \log (1 - h_\theta(x^{(i)}))] + \frac{\lambda}{2m}\sum_{j=1}^n \theta_j^2\tag{DIS}\label{eq:dis}
$$

## Prism

### Java

```java
@ShellComponent
@Slf4j
public class AudioSine {
    final int SAMPLE_RATE = 44100;

    @ShellMethod(value = "Play a sine  in a precalculated buffer")
    public void sine(@ShellOption(value = "-o") String outputDevice) {
        AudioDeviceManager m = new AudioDeviceManager();
        m.collectDevices();
        m.getOutputs().stream().filter(d -> d.getName().equals(outputDevice))
            .findFirst()
            .ifPresentOrElse(this::playSine, () ->log.error("Device not found:" + outputDevice));
    }
}		
```

### Json

```json
{
	"age": 13
	age: 14
}
```

### bash

```bash
#!/bin/sh

echo "Hello world !"
```

## Alerts


> [!NOTE]
> An alert of type 'note' using global style 'callout'.

> [!TIP]
> An alert of type 'tip' using global style 'callout'.

> [!WARNING]
> An alert of type 'warning' using global style 'callout'.

> [!ATTENTION]
> An alert of type 'attention' using global style 'callout'.
