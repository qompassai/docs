<!-- ~/.GH/Qompass/Docs/tuned/README.md -->
<!-- ---------------------------------- -->
<!-- Copyright (C) 2025 Qompass AI, All rights reserved -->

<h2> Energy saving Tuning </h2>

<h3> Options to choose from </h3>


- Tuned ( generally better for servers)

--- OR

- tlp (generally better for laptops & more granular)

--- NOT BOTH

* For Tuned

```bash
sudo systemctl --enable tuned --now
```
- See what the profiles are

```bash
sudo tuned-adm list
```

<h4> Profiles </h4>

```bash
- balanced
- powersave
- latency-performance
- throughput-performance
- virtual-guest
- desktop
- laptop-ac-powersave
```

<h4> Max powersave </h4>

```bash
sudo tuned-adm profile laptop battery-powersave
```

<h4> Desktop/moderate savings </h4>

```bash
sudo tuned-adm profile powersave
```

- OR

```bash
sudo tuned-adm profile desktop
```
