# Custom descriptions

Genesis allows you to add description texts to gear, spells and other data types. These show up in the application and on the optional PDF export pages for your character. By doing so, you can have all spell or qualitity descriptions for your character exported in a PDF.

### Locate the data directory

The directory where Genesis stores your data can be found in the Genesis settings on the first page.

### Create a `custom/shadowrun6/fallback-help.properties` file

In your data directory should be a subdirectory named `custom`. Within create a subdirectory named `shadowrun6`. There create a file named `fallback-help.properties`.

On Windows this might look like: `C:\Users\Stefan\rpgframework\custom\shadowrun6\fallback-help.properties`

On Linux this might look like `/home/stefan/rpgframework/custom/shadowrun6/fallback-help.properties`

### Write your text

To add a description to an item existing in Genesis, you must know the correct key. The key is always in the format `<type>.<identifier>.desc` - e.g. `item.gas-vent-system.desc`. To learn the correct types and identifiers look at the [regular properties](https://bitbucket.org/rpgframework/shadowrun-6/src/master/Shadowrun6_Data/src/main/resources/org/prelle/rpgframework/shadowrun6/data/core/i18n/core.properties "https://bitbucket.org/rpgframework/shadowrun-6/src/master/Shadowrun6_Data/src/main/resources/org/prelle/rpgframework/shadowrun6/data/core/i18n/core.properties") file.

E.g.

```properties
quality.astral_chameleon.desc=Hello World
quality.toxin_resistance.desc=Goodbye World
```
