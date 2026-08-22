# Release Notes Q4 2025

## Overview

This document summarizes the key updates, improvements, and bug fixes released in Q4 2025 for the Atea Managed Public Cloud.

## New Features

- **Monitoring version 2:** We can now create custom parameters per alarm and completely custom alarms.
- **New patch dashboard:** A new dashboard now displays data about the patching of virtual machines.
- **VM and VMSS supported:** Both VM and VMSS are now supported. Documentation for the alarms can be found in our public repository.
- **Native network components are supported:** The most commonly used network components are now supported by the service.

## Improvements

- **Improved cost dashboard:** The cost dashboard now provides a better overview, eliminating the need to review costs subscription by subscription.
- **Optimized alerts:** We have made multiple improvements, deletions, and consolidations of alerts.
- **New version of Terraform:** With version 2 of the monitoring code, we now use the latest version of Terraform.

## Bug Fixes

- **Wrong priority on HTTP errors:** HTTP error 4xx was incorrectly set as P2, while HTTP error 5xx was set as P3. These priorities have now been swapped.
- **Reprioritization of alarms:** We have updated the prioritization of alarms in our repository.
- **Moved a few services:** Some services have been moved from Platform to Network to better align with Microsoft's categorization.

## Known Issues

- **Service health alerts:** There is a known issue with the Terraform Provider that prevents us from changing the priority of health alerts.
- **Auto-resolving health alerts:** Health alerts do not auto-resolve, making it harder to maintain accurate status information in our dashboards.
