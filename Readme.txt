A-Frame Builder v49.5 (sq/ft Update)

A web-based tool for planning and visualizing the loading of stone slabs onto A-frame trucks with intelligent distribution, drag-and-drop rearrangement, and comprehensive validation.

Overview
This application helps logistics teams optimize truck loading by

Automatically distributing slabs across A-frame racks based on weight and constraints

Providing visual drag-and-drop interface for manual adjustments

Validating load safety (weight limits, balance, customer restrictions, slab stacking rules)

Generating printable loading manifests with customer stop information

Features
Core Functionality

CSV Import: Process load reports with stop numbers, customer info, and slab details.

Intelligent Distribution: Automatically assigns slabs to frames considering:

Weight limits (per side and total)

Thickness constraints (CM limits)

Customer Restrictions (back-only requirements)

Slab Stacking Rules (sq/ft restriction)

Load Balancing: Balances load between driver/passenger sides.

Interactive Controls

Drag & Drop: Move slabs between frames and sides.

Manual Slab Addition: Add custom slabs with stop insertion/renumbering.

Frame Management: Remove empty frames from layout.

Layout Reset: Restore original automated distribution.

Validation & Safety

Real-time Alerts: Notifications for overloads, imbalances, and placement violations.

Customer Restrictions: Enforces back/front placement requirements.

Weight Calculations: Automatic weight estimation based on slab size and thickness.

NEW: Slab SQ/FT Restriction: Alerts if a large slab (e.g., > 47 sq/ft) is placed on top of a restricted sq/ft base slab.

Output

Visual Truck Layout: Color-coded representation of loaded frames.

Printable Manifest: Generates a clean, organized printout with all customer and slab details.

Usability
Layout

Frames are arranged vertically, with driver and passenger sides clearly labeled.

Slabs display Stop Number, Locator, Description, and Lot information.

Keyboard Shortcuts

Print: Browser print shortcut (Ctrl+P) or on-screen print button

Reset: Reset Layout button to restore automated distribution

Drag & Drop: Click and drag slabs between frames

Browser Compatibility

Chrome (recommended)

Firefox

Safari

Edge

Note: Requires modern browser with ES6+ support and drag/drop API.

Technical Details

Libraries Used: Tailwind CSS, PapaParse, Font Awesome, Google Fonts (Roboto).

Data Persistence: All data exists in browser memory (no server storage). Refresh/close browser to clear current load. Print or save PDF for permanent records.

Troubleshooting Common Issues

CSV won't upload: Check column headers match expected format.

Slabs not distributing: Verify stop numbers are numeric and > 0.

Drag/drop not working: Ensure you're dragging the entire slab bar, not just text.

Print layout broken: Use the print button rather than browser print for optimized formatting.

Validation Errors

OVERLOADED: Total frame weight exceeds safe limit.

Width Exceeded: Too many CM on one side of frame.

Imbalanced: Weight difference between sides exceeds threshold (1,500 lbs default, 4,500 lbs for Metal Aframe Truck).

Restriction Violation: Back-only customer placed on front frame.

SQ/FT SLAB VIOLATION (NEW): Slabs larger than the restricted size cannot be stacked on top of a base sq/ft slab.

Version History

v49.5 (Current) - SQ/FT Update

Updated Metric: All mentions of "inches" for slab size restriction replaced with "sq/ft".

Added SQ/FT Slab Restriction: Implements a safety rule to prevent placing large slabs on top of a restricted sq/ft base slab.

Visual Enhancement: Restricted sq/ft slabs are now highlighted in light green with a badge for easy identification.

v49.4 (Previous)

Added manual slab deletion capability.

Enhanced drag/drop visual feedback.

Improved print formatting.

Fixed stop insertion logic.

Previous versions included foundational distribution algorithm, CSV processing, and basic UI.