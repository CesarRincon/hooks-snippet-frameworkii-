# Snippets Framework II

Es una pequeña herramienta para agilizar el proceso de escribir codigo en el framework II

# Snippets

### Components

- Components from [official docs](htthttps://rn-framework-docs.vercel.app/docs/category/styleguide) are added with component name as prefix.

### Hooks

|   Prefix | Method                                          |
| -------: | ----------------------------------------------- |
| `hookst` | `Create a basic template of the hook structure` |
|   `hook` | `Create the basic structure of a hook.`         |

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

### Components

|                       Prefix | Method                                                                           |
| ---------------------------: | -------------------------------------------------------------------------------- |
|                  `rich-text` | `Create a basic template of the rich-text component structure`                   |
|                       `link` | `Create a basic template of the link component structure`                        |
|                     `linkCh` | `Create a basic template of the link with children component structure`          |
|                     `linkCh` | `Create a basic template of the link with children component structure`          |
|                    `grid-sv` | `Create a basic template of the grid with mode scroll-view component structure`  |
|                     `grid-v` | `Create a basic template of the grid with mode view component structure`         |
|                       `icon` | `Create a basic template of the icon component structure`                        |
|              `button-submit` | `Create a basic template of the form button component structure`                 |
|                  `input-otp` | `Create a basic template of the form input type otp component structure`         |
|                `input-email` | `Create a basic template of the form input type email component structure`       |
|             `input-password` | `Create a basic template of the form input type password component structure`    |
|          `schema-validation` | `Create a basic template of the form validation component structure`             |
| `schema-validation-password` | `Create a basic template of the form validation of password`                     |
|          `validate-required` | `Create a basic template of the form validation of required value `              |
|               `validate-min` | `Create a basic template of the form validation of minimum characters value`     |
|      `validate-match-number` | `Create a basic form validation template of at least one numeric character`      |
|       `validate-match-mayus` | `Create a basic form validation template of at least one uppercase character`    |
|       `validate-match-minus` | `Create a basic form validation template of at least one character in lowercase` |
|       `validate-match-minus` | `Create a basic template of the form component structure`                        |

### Examples

### `rich-text`

```json
{
  "componentName": "rich-text",
  "props": {
    "text": "",
    "style": ""
  }
}
```

### `link`

```json
{
  "componentName": "link",
  "props": {
    "href": "",
    "text": "",
    "style": ""
  }
}
```

### `linkCh`

```json
{
  "componentName": "link",
  "props": {
    "href": "",
    "text": "",
    "style": ""
  },
  "children": []
}
```

### `grid-sv`

```json
{
  "componentName": "grid",
  "props": {
    "container": true,
    "direction": "row",
    "justifyContent": "flex-start",
    "alignItems": "flex-start",
    "flex": 1,
    "mode": "scroll-view",
    "showsVerticalScrollIndicator": false,
    "showsHorizontalScrollIndicator": false,
    "style": ""
  },
  "children": []
}
```

### `grid-v`

```json
{
  "componentName": "grid",
  "props": {
    "container": true,
    "direction": "row",
    "justifyContent": "flex-start",
    "alignItems": "flex-start",
    "flex": 1,
    "mode": "view",
    "style": ""
  },
  "children": []
}
```

### `icon`

```json
{
  "componentName": "store-icons",
  "props": {
    "name": "",
    "style": ""
  }
}
```

### `button-submit`

```json
{
  "componentName": "store-form.submit",
  "props": {
    "buttonText": "",
    "style": ""
  }
}
```

### `input-otp`

```json
{
  "componentName": "store-form.input",
  "props": {
    "name": "",
    "variant": "otp-code",
    "placeholderTextColor": "",
    "style": ""
  }
}
```

### `input-email`

```json
{
  "componentName": "store-form.input",
  "props": {
    "name": "email",
    "placeholder": "",
    "style": ""
  }
}
```

### `input-password`

```json
{
  "componentName": "store-form.input",
  "props": {
    "name": "password",
    "isPassword": true,
    "placeholder": "",
    "iconName": "",
    "style": ""
  }
}
```

### `schema-validation`

```json
"schemaValidation": [
	{
		"id": "",
		"type": "text",
		"validationType": "string",
		"validations": []
	}
]
```

### `schema-validation`

```json
"schemaValidation": [
	{
		"id": "",
		"type": "text",
		"validationType": "string",
		"validations": []
	}
]
```

### `schema-validation-password`

```json
"schemaValidation": [
	{
		"id": "password",
		"type": "text",
		"validationType": "string",
		"validations": [
			{
				"type": "required",
				"params": ["Este campo es requerido"]
			},
			{
				"type": "min",
				"params": [
				6,
				"Tu contraseña debe contener mínimo 6 digitos"
				]
			},
			{
		 		"type": "matches",
		 		"params": ["/^.*[0-9].*$/", "1 número"]
			},
			{
		 		"type": "matches",
		 		"params": ["/^.*[a-z].*$/", "1 minúscula"]
			},
			{
				"type": "matches",
				"params": ["/^.*[A-Z].*$/", "1 mayúscula"]
			}
		]
	}
]
```

### `validate-required`

```json
{
  "type": "required",
  "params": ["Este campo es requerido"]
}
```

### `validate-required`

```json
{
  "type": "required",
  "params": ["Este campo es requerido"]
}
```

### `validate-min`

```json
{
  "type": "min",
  "params": [6, "Tu contraseña debe contener mínimo X digitos"]
}
```

### `validate-match-number`

```json
{
  "type": "matches",
  "params": ["/^.*[0-9].*$/", "1 número"]
}
```

### `validate-match-mayus`

```json
{
  "type": "matches",
  "params": ["/^.*[A-Z].*$/", "1 mayúscula"]
}
```

### `validate-match-min`

```json
{
  "type": "matches",
  "params": ["/^.*[a-z].*$/", "1 minúscula"]
}
```

### `form`

```json
{
  "componentName": "store-form",
  "props": {
    "context": [],
    "mode": "onChange",
    "scrollView": true,
    "parseInput": {
      "to": {}
    },
    "style": ""
  },
  "children": []
}
```

**Enjoy!**
