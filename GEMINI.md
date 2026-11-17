# SoloCatalog

These tools read an original (OEM) car parts catalogue: part numbers and exploded diagrams. No account is needed and every tool only reads.

- With a VIN: `decode_vin`, then `search_parts` with the VIN and a part name ("front brake pads") or a part number.
- Without a VIN: `find_models` with the brand and model words, then `search_parts` or `list_diagrams` with the model it returns.
- `list_diagrams` then `get_diagram_parts` to read one assembly with positions, quantities and fitment notes.
- `lookup_part_number` when the user already has a number.

Quote part numbers exactly as returned and keep the link to the vehicle or diagram on solocatalog.com. Results found without a VIN are candidates for every build of that model: tell the user to confirm fitment with the VIN before ordering. The catalogue has no prices, stock or repair instructions; do not make them up.
