# This schema repo is now deprecated

Please refer to the official homebrew schema which was built with support from this project:

```json
{
    "$schema": "https://raw.githubusercontent.com/TheGiddyLimit/homebrew/master/_schema-fast/homebrew.json"
}
```

Either use the 'fast' schema to validate live in your IDE; or run the full validation script which is available here:

<https://raw.githubusercontent.com/TheGiddyLimit/homebrew/master/_test/test-json.js>

## Final Site Version Compatibility and Provenance

This schema repo is currently updated to support version `1.142.0` of the site.

This schema is built from the original 5eTools Site Schema which can be found [here](https://github.com/5etools-mirror-1/5etools-mirror-1.github.io/tree/master/test/schema).

It further adapts the [main schema file](https://github.com/TheGiddyLimit/homebrew/blob/master/schema.json) from the homebrew repository that it aims to fully lint, which is available [here](https://github.com/TheGiddyLimit/homebrew).

## How to use it with VSCode

- Download the folder with the schema
- Put it into a another folder in your VS Code Workspace
- Go to Settings and search for Schema
- Edit the settings.json for the JSON: Schemas setting
- Put this into your `"json.schemas"` array with your correct paths:

```json
{
    "fileMatch": [
        "*.json"
    ],
    "url": "../5etools-Homebrew-Schema/schema.json"
}
```

Alternatively you can simply add the following line to your homebrew file, though this is not advised and setting up your environment is preferred:

```json
{
    "$schema": "https://raw.githubusercontent.com/revilowaldow/5eSchema/main/5etools-Homebrew-Schema/schema.json"
}
```

Every json file you make in this workplace folder now will use this schema.  
If something's missing or wrong let me know on Discord.
