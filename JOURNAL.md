## My journal for this Highway!
# Day 1: Idea

I bought a broken e-scooter (by broken, I mean completely melted electronics) and decided to rebuild it. I got a new controller and display board, but no way to interface them easily or charging the battery.
I then realized: I have tons of 18650 batteries laying around. Why not use them to boost my scooter's voltage, and fix all the problems I'm having on a single board? So this module should feature:
- BMS for the extra 12V DIY battery pack
- USB Type-C connector to interface with the bluetooth dashboard (both the dashboard and the controller have finnicky JST connectors, I'm replacing them for some solid, modern USBC)
- Charger for the batery (The scooter's charger is 42V. Should I charge the extra 12V battery in parallel by stepping-down those 42? I believe a boost converter from 42 to 54.6 will be much more reasonable.)
- Overcurrent charge protection (in case the charging port gets shorted)
- - _Along with as much protections I can think of_![20250518_161551](https://github.com/user-attachments/assets/665c4280-d442-4ae1-a95f-930a86e57e24)

# Day 2: Schematic Layout

I began the schematic by laying out a few functional blocks. 
![image](https://github.com/user-attachments/assets/1e05587f-4712-4b63-b41c-8d8eb69bd59e)
