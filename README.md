# Week Number Plugin for TRMNL

This plugin displays the current week number on your TRMNL device. It features a dynamic background that acts as a progress bar, visualizing how much of the year has passed.

## Features

-   **Current Week Display**: Clearly shows the current week number.
-   **Year Progress Bar**: The background fills up from left to right as the year progresses.
-   **High Contrast**: Uses `mix-blend-mode: difference` to ensure the text remains legible (inverting colors) as the background fills behind it.
-   **Responsive Layouts**: Supports all TRMNL layouts:
    -   Full
    -   Half Horizontal
    -   Half Vertical
    -   Quadrant

## How it Works

The plugin uses Liquid templating to calculate the current week number from the system time (`trmnl.system.timestamp_utc`). It then calculates the percentage of the year passed (current week / 52) and uses this percentage to set the width of the background overlay.

## Installation

1.  Create a new private plugin on your TRMNL dashboard.
2.  Copy the contents of the `.liquid` files into the corresponding layout sections in the Edit Plugin view.
3.  Copy the contents of `shared.liquid` into the "Shared" tab within the CSS/JS section.

## Configuration

No special configuration is required. The plugin automatically uses the current UTC timestamp provided by the TRMNL system.
