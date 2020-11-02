# URL Schemes

Taio supports launching functionalities using URL schemes, which can make your workflow more flexible.

> If your scenario is not supported, please let us know and we can improve.

## Save Clipboard

```
taio://clips?action=save
```

## Copy to Clipboard

```
taio://clips?action=copy&text=text
```

## Clear All Clips

```
taio://clips?action=clear
```

> Be careful with this, it clears all clips without asking for confirmation.

## Create A New File

```
taio://editor?action=new
```

## Open A File in The Editor

```
taio://editor?action=open&path=path&location=0
```

`location` 0: local files, 1: iCloud Drive files.

## Import Actions

```
taio://actions?action=import&url=url
```

## Run Actions

```
taio://actions?action=run&name=name&input=input
```

## URL Encoding

Note that, URL parameters should be URL encoded, for example:

```
taio://actions?action=import&url=https%3A%2F%2Ftaio.app%2Fdemo.taioactions
```

The original text for `url` is `https://taio.app/demo.taioactions` (It's a pseudo link just for example), without URL encoding, the parameter will not be correctly extracted.