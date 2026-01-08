# Universal Printer Supply Levels by SNMP
As long as your MFP follows the Printer MIB standard, this template will discover all installed "Supplies" in your MFP via SNMP. "Marker Supplies" is the term used in the Printer MIB for toner, ink, and other consumable substances that make a mark on whatever you're printing on.

## What's provided
Item prototypes use the "current" and "max" values provided by SNMP to calculate the remaining amount in a percentage. Simple graph prototypes included.

Alert prototypes provide an info-level alert when the "low" threshold is crossed, and a warning-level alert when the "critical" threshold is crossed. These are 5% and 0% by default, and are adjustable with provided macros.

## Additional tweaking
Depending on how your printer uses the Supplies table, you may end up with unused or duplicate items discovered. Every discovered item will have its SNMP index as part of the item key (e.g. supply.type.[5] for the supply at SNMP Index 5) - Any indices you wish to filter out of discovery, I've provided macros to do so.

You can learn more about the Printer MIB by searching for it on your favorite search engine. It's old, hasn't changed, and is widely used and documented.

## Credits
Author: Mick Swanson
