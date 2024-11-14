
# Zabbix Template for Ekinops DWDM Equipment

This repository contains a custom Zabbix template designed for monitoring Ekinops Dense Wavelength Division Multiplexing (DWDM) equipment via SNMP.

## Overview

This is a custom Zabbix template built specifically for Ekinops DWDM devices. The template uses SNMP to monitor key performance metrics and operational statuses for Ekinops equipment. **Please note that this template is provided "as-is," and its use is at your own risk.** There is no warranty or official support provided for this template, so be sure to thoroughly test it in your environment before deploying to production.

## Features

The template includes:

- **Key Performance Metrics:** Essential metrics for monitoring the health and performance of Ekinops DWDM equipment.
- **Standard Triggers:** Predefined triggers for alerting on significant status changes or performance issues.
- **Customizable Options:** You may add, modify, or remove items and triggers to meet specific monitoring needs.

## Requirements

- **Zabbix Server:** Tested with Zabbix version 5.x and higher.
- **SNMP Access:** Requires SNMP access to the Ekinops DWDM device.
- **Ekinops MIBs:** Ensure that relevant Ekinops MIB files are available and loaded for accurate monitoring.

## Installation

1. **Import the Template:**
   - In Zabbix, navigate to **Configuration > Templates**.
   - Click on **Import** and select the `zbx_ekinops_dwdm_snmp-template.yaml` file.

2. **Link the Template to a Host:**
   - Assign the template to the host that corresponds to your Ekinops DWDM device in Zabbix.

3. **Configure SNMP Community:**
   - Ensure that the SNMP community string is configured correctly on the host settings to allow successful SNMP polling.

## Usage

Once linked to the Ekinops device, Zabbix will begin polling according to the template's configuration. You can view collected data under the **Monitoring** tab in Zabbix and set up custom alerts based on collected metrics and trigger configurations.

## Customization

Feel free to modify the template to better suit your monitoring requirements. Common modifications include:

- Adjusting the polling intervals for specific items.
- Customizing thresholds on triggers.
- Adding or removing metrics as required.

## Troubleshooting

If you encounter issues with the template:

- Ensure that SNMP access is properly configured on the Ekinops device.
- Verify that the correct SNMP version and community string are configured in Zabbix.
- Confirm that necessary Ekinops MIB files are accessible.

## Contributing

Contributions to improve this template are welcome. Feel free to submit a pull request or open an issue if you have suggestions for enhancements or encounter issues.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Disclaimer:** This template is provided without warranty of any kind. Its use is entirely at your own risk. The author and contributors are not responsible for any damages resulting from the use of this template.
