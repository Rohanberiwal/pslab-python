# PSLab Python Library

The Python library for the [Pocket Science Lab](https://pslab.io) from FOSSASIA.

[![Build Status](https://github.com/fossasia/pslab-python/actions/workflows/workflow.yml/badge.svg)](https://github.com/fossasia/pslab-python/actions/workflows/workflow.yml)
[![Gitter](https://badges.gitter.im/fossasia/pslab.svg)](https://gitter.im/fossasia/pslab?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ce4af216571846308f66da4b7f26efc7)](https://www.codacy.com/app/mb/pslab-python?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fossasia/pslab&amp;utm_campaign=Badge_Grade)
[![Mailing List](https://img.shields.io/badge/Mailing%20List-FOSSASIA-blue.svg)](https://groups.google.com/forum/#!forum/pslab-fossasia)
[![Twitter Follow](https://img.shields.io/twitter/follow/pslabio.svg?style=social&label=Follow&maxAge=2592000?style=flat-square)](https://twitter.com/pslabio)


This repository hosts the Python library for seamless communication with the Pocket Science Lab open hardware platform (PSLab). Through this library, users can interact with PSLab using straightforward Python code. Additionally, the Python library serves as a vital backend component for the PSLab GUI.

PSLab aims to create an Open Source hardware device, open on all layers, alongside software applications tailored for experiments by educators, students, and scientists. The pocket lab provides various measurement tools, including an oscilloscope, waveform generator, logic analyzer, programmable voltage and current source, and a component for controlling robots with up to four servos.

For more information see [https://pslab.io](https://pslab.io).

## Features 
Features
Highlight the key features and capabilities of the PSLab Python Library, such as:
Communication with PSLab for various experiments.
Integration with the PSLab GUI.
Support for measurement tools including an oscilloscope, waveform generator, logic analyzer, programmable voltage, current source, and servo control.
Open-source nature and collaboration with the PSLab project.

## Buy

* You can get a Pocket Science Lab device from the [FOSSASIA Shop](https://fossasia.com).
* More resellers are listed on the [PSLab website](https://pslab.io/shop/).

## Installation

pslab-python can be installed from PyPI:

	$ pip install pslab

**Note**: Linux users must either install a udev rule by running 'pslab install' as root, or be part of the 'dialout' group in order for pslab-python to be able to communicate with the PSLab device.

**Note**: If you are only interested in using PSLab as an acquisition device without a display/GUI, only pslab-python needs to be installed. If you would like a GUI, install the [pslab-desktop app](https://github.com/fossasia/pslab-desktop) and follow the instructions of the Readme in that repo.


## Validate installation

1. Plug in the PSLab device and check that both the LEDs light up.
2. The following piece of code should run without errors:
```
from pslab import ScienceLab
psl = ScienceLab()
capacitance = psl.multimeter.measure_capacitance()
print(capacitance)
```

## Communication

* If you encounter any bugs, please file them in our [issue tracker](https://github.com/fossasia/pslab-python/issues).
* You can chat with the PSLab developers on [Gitter](https://gitter.im/fossasia/pslab).
* There is also a [mailing list](https://groups.google.com/forum/#!forum/pslab-fossasia).

Wherever we interact, we strive to follow the [FOSSASIA Code of Conduct](https://fossasia.org/coc/).

## Contributing

See [CONTRIBUTING.md](https://github.com/fossasia/pslab-python/blob/development/CONTRIBUTING.md) to get started.

## License

Copyright (C) 2014-2021 FOSSASIA

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 3.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.

## Social Media and Community Engagement
[![Twitter Follow](https://img.shields.io/twitter/follow/pslabio.svg?style=social&label=Follow&maxAge=2592000?style=flat-square)](https://twitter.com/pslabio)
[Mailing List](https://groups.google.com/forum/#!forum/pslab-fossasia)
[Gitter Chat](https://gitter.im/fossasia/pslab)

## Communication and Support
Encourage users to report any bugs they encounter through the issue tracker. Highlight the available support channels, such as the Gitter chat and the mailing list.

