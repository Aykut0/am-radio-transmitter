# AM Radio Transmitter

Course project for ELEC 310 (Analog Electronics) at Koç University. A single-transistor AM transmitter built from discrete parts, simulated in LTspice and tested on the bench.

![Modulated sine wave on the oscilloscope](docs/images/scope_modulated_sine.jpg)

An LC tank (an inductor and a variable capacitor) sets the carrier frequency, tunable around the AM band; the demo ran at about 1.3 MHz. The audio signal joins the carrier at the transistor's base, so it changes the carrier's amplitude, and a pi filter after the transistor cleans up the output before the antenna. I started from the single-transistor transmitter on [LEAP](https://leap.tardate.com/radio/am/singletransistortransmitter/), then re-derived the biasing and simulated each stage before building it.

![LTspice schematic](docs/images/ltspice_schematic.png)

| Carrier only (simulation) | Carrier and audio (simulation) |
|---|---|
| ![Carrier only](docs/images/sim_carrier_only.png) | ![Modulated output](docs/images/sim_modulated.png) |

| Modulated audio on the scope | Breadboard build |
|---|---|
| ![Modulated audio](docs/images/scope_audio.jpg) | ![Breadboard](docs/images/breadboard.jpg) |

## Files

```
ltspice/   LTspice schematics: carrier only, audio only, carrier and audio
docs/      project report and images
```

Open any `.asc` file in LTspice and run the transient simulation.

---

Yaşar Aykut Altuntop · Koç University · [LinkedIn](https://linkedin.com/in/aykutaltuntop) · [GitHub](https://github.com/Aykut0)
