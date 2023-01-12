### Energy Manager

This project aims at improving the energy management natively provided by commercial devices in the field of solar thermal and photovoltaic power solutions.

The proposed application will ultimately deliver the following services and functions:
+ collect, store and display data from sensors such as solar and thermal probes, device counters;
+ control devices such as solar pumps and valves, heating system, electrical inverters and battery chargers;
+ collect external data such as weather forecasts[^first] and the number of people expected in the building;
+ use these control systems and internal/external data to optimize the production and storage of solar thermal and photovoltaic energy;
+ provide tools to cross-analyze collected data, power management decisons and results obtained;
+ help with energy system sizing and improve decision algorithms.

This project also intends to implement up-to-date methods and tools:
+ Scrum and CI/CD approaches and tools;
+ container-based microservice architecture (data flows, data storage, device control, user interface...);
+ artificial intelligence such as Machine Learning (data analysis, decision algorithms...).

This application will be the subject of a proof of concept in the following configuration:
+ combined[^second] solar system: solar thermal collectors (18 m²) + PWM solar pump + 1000l tank + 3 temperature probes + 3 way-valve + system controller + Resol Vbus/Ethernet interface.
+ photovoltaic system: solar array (12 m²) + charge controller + inverter[^third] + 12V battery storage + Victron VE.Direct/USB interface.
+ Linux server interfacing with solar system interfaces and hosting Docker containers.

[^first]: a quite sunny weather forecast in summer would typically result in limiting the use of carbon energies to produce hot water the night before.
[^second]: combined solar (thermal) systems provide both hot water (primarily) and central heating (partially).
[^third]: inverter usage includes powering both thermal and photovoltaic systems in order to have them self sufficient.
