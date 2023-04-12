# Snippets Framework II

Es una pequeña herramienta para agilizar el proceso de escribir codigo en el framework II

# Snippets

### Components

- Components from [official docs](htthttps://rn-framework-docs.vercel.app/docs/category/styleguide) are added with component name as prefix.

### Hooks

|      Prefix | Method                                                                      |
| ----------: | --------------------------------------------------------------------------- |
|      `hookst` | `Create a basic template of the hook structure`                                                 |
|     `hook` | `Create the basic structure of a hook.`                                          |

### Examples

### `hookst`

```json
{
    "hooks": [
        {
            "name": "", 
            "fetchOptions": { 
                "url": "",
                "query": ""
            },
            "componentType": "omni-hook", 
            "exec": [ 
                {
                    "name": "",
                    "function": "",
                    "params": []
                }
            ] 
        }
    ]
}
```

### `hook`

```json
{
    "name": "", 
    "fetchOptions": { 
        "url": "",
        "query": ""
    },
    "componentType": "omni-hook", 
    "exec": [ 
        {
        "name": "",
        "function": "",
        "params": []
        }
    ] 
}
```
**Enjoy!**