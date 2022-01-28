# Bitburner-tools

A collection of personal scripts used in the game *Bitburner*. Working as of version **v1.4.0** on Steam.

## Component Scripts

 * `doGrow.ns`
 * `doHack.ns`
 * `doWeaken.ns`
 * `flag-sys-restart.ns`
 * `flag-sys-settings.ns`
 * `flag-sys-update.ns`
 * `flag-received.ns`

## sys-manager-2.ns (heavyweight - 37.85GB RAM)

### Current Features:
 * Automatic server discovery and rooting
 * Automatic hacking, growing and weakening
 * Hacks servers in close-to optimal order using available resources
 * Optimally hacks servers whilst wasting minimal resources
 * Can run in silent mode (no terminal messages or toasts)
 * Can run in greedy mode (prefer servers with more available money)
 * Can run in very greedy mode (only hack, don't grow or weaken)
 * Can be flagged to update servers manually (using asynchronous flagging procedures)
 * Handles additional servers and updating of RAM on known servers.
 * Automatic contract detection and solving
 * Flag for mid-runtime setting updates.
 
### Current TODO:
 * Improved Logging V2
 * Asset Tracking (generated income, reputation etc.)
 * Stock Trading (with 4S and without incorporated) to increase assets using a simple moving average
 * Automatic server purchasing
 * Stepped thresholds for varying progression stages (script works early to late game with no interference through defined thresholds)

## sys-manager.ns (lightweight - 12.60GB RAM)

Same as above (heavyweight version) but less features - no contract solving, less effective resource distribution, less flagging options etc.

## basic-server-info.ns (1.80GB RAM)

Prints the specified server's maximum money and available money (along with a percent of max money available). For simple manual inspection.

## purchase-server.ns (4.05GB RAM)

A simple utility script for automatically purchasing a server of the specified size.

## killall-bfs.ns (2.35GB RAM)

A simple utility that performs a breadth-first search for servers within a certain connection depth of the host server, killing all running processes on all found servers. Used to quickly kill distributed scripts.