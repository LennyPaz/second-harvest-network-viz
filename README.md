# Second Harvest Network Visualization

An interactive 3D visualization of the enterprise LAN designed for **Second Harvest of the Big Bend**, a food bank nonprofit in Tallahassee, FL. Built for LIS 4482 (Introduction to Networks and Telecommunications).

## What it shows

A three-tier network topology (edge router → core switch → access switches → endpoints) serving a 41,000 sq ft warehouse facility. Devices are organized into VLANs by department and function, and animated traffic flows between them illustrate how packets traverse the network.

## VLANs

| VLAN | Name | Subnet | Purpose |
|---|---|---|---|
| 10 | Admin | 10.10.10.0/24 | Executive, HR, Finance |
| 20 | Operations | 10.10.20.0/24 | Warehouse management, logistics |
| 30 | Programs | 10.10.30.0/24 | Child nutrition, senior programs |
| 40 | Development | 10.10.40.0/24 | Fundraising, marketing |
| 50 | Warehouse Wireless | 10.10.50.0/24 | Mobile scanners |
| 60 | Guest | 10.10.60.0/24 | Volunteer WiFi (isolated) |
| 70 | Servers | 10.10.70.0/24 | DC/DNS, File, Print, App |
| 80 | VoIP | 10.10.80.0/24 | IP phone system |
| 90 | IoT | 10.10.90.0/24 | Security cameras, sensors |

## How to run

It's a single self-contained HTML file. No build tools, no install.

1. Clone or download this repo.
2. Open `second-harvest-network.html` in Chrome.

That's it. Three.js loads from CDN.

## Author

Lenny Paz — Florida State University, LIS 4482
