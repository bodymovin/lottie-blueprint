# Abstract

The Lottie Blueprint Format is not intended to validate that a lottie json file is a valid Lottie animation. Its purpose is to work as a template validator for lottie animations. As an example, it will validate that there are two shape layers in the animation, or whether assets are no larger than a certain width / height.

## Example

```json
{
  "type": "blueprint",
  "value": "dt",
  "text": "Dynamic Text",
  "parser":{
    "slots": {
      "entries": [
        {
          "name": "Rotation",
          "type": "regex",
          "count": {
            "operation": ">=",
            "value": 1
          },
          "property": "rotation"
        },
        {
          "name": "Scale",
          "type": "regex",
          "count": {
            "operation": ">",
            "value": 0
          },
          "property": "scale"
        },
        {
          "name": "Opacity",
          "type": "regex",
          "count": {
            "operation": ">=",
            "value": 1
          },
          "property": "opacity"
        },
        {
          "name": "ImageSource",
          "type": "regex",
          "count": {
            "operation": ">=",
            "value": 1
          }
        }
      ]
    },
    "layers": {
      "count": {
        "operation": "===",
        "value": 1
      },
      "entries": [
        {
          "type": 0,
          "count": {
            "operation": "===",
            "value": 3
          }
        }
      ]
    },
    "assets": {
      "count": {
        "operation": ">",
        "value": 0
      }
    }
  }
}
```