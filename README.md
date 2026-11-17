# SoloCatalog for Gemini CLI

Look up original (OEM) car part numbers and exploded parts diagrams from Gemini CLI, from the same catalogue as [solocatalog.com](https://solocatalog.com). No account or API key is needed.

## Install

```bash
gemini extensions install https://github.com/alik472/solocatalog-gemini-extension
```

That is all: there is no account, sign-in or API key.

## What you can ask

- Find the oil filter part number for VIN WVWZZZAUZGW180767.
- Which front brake pads fit a 2018 Toyota Camry?
- List the cooling system diagrams for this VIN and show the parts of the water pump one.
- What is Toyota part number 11011-25010 and where is it used?

## Tools

| Tool | What it does |
| --- | --- |
| `decode_vin` | Identifies a vehicle from its VIN or Japanese frame number and says whether its catalogue can be searched. |
| `search_parts` | Finds OEM part numbers for a vehicle by part name or by a full or partial part number. |
| `find_models` | Finds a parts catalogue by brand and model words when there is no VIN. |
| `list_diagrams` | Lists the exploded diagrams (assemblies) of a vehicle. |
| `get_diagram_parts` | Every part of one diagram with number, name, position, quantity and fitment notes. |
| `lookup_part_number` | What a part number is and the models and diagrams where it is listed. |

## Good to know

- Covered brands: Toyota, Lexus, Nissan, Infiniti, Honda, Mazda, Mitsubishi, Subaru, Hyundai, Kia, BMW, Mercedes-Benz, Volkswagen, Audi, Skoda, SEAT, Opel/Vauxhall, Ford (Europe), Land Rover and Chevrolet. Coverage depends on the vehicle, market and catalogue release.
- Part numbers and diagrams only: no prices, stock, ordering or repair instructions.
- Results found without a VIN are candidates for every build of that model. Confirm fitment with the VIN before ordering.
- There is a daily request allowance without an account. When it is used up the tools say so, and the same catalogue stays searchable in the browser.
- SoloCatalog is an independent catalogue and is not affiliated with or endorsed by any vehicle manufacturer.

## Other MCP clients

The extension only points Gemini CLI at SoloCatalog's hosted MCP server (streamable HTTP):

```
https://solocatalog.com/mcp
```

Any MCP client that supports remote servers can use the same address. It needs no authentication.

## Links

[Website](https://solocatalog.com) · [Privacy](https://solocatalog.com/privacy) · [Terms](https://solocatalog.com/terms) · [Contact](https://solocatalog.com/contact)

## License

The files in this repository are released under the MIT License. The SoloCatalog service itself is covered by its terms.
