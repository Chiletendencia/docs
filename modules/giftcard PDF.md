# Explanatory Videos
- [Video explicando a Marko](https://youtu.be/NyTUSNqdaOE)
- [Allow PDF storage resources from prod and dev environments](https://youtu.be/YBzGHz1aiCs)

# Technical details
## TWO_IMAGES
    Internally, it consists in a table with a single row and two cells with an image each
        
            Page
            ▲      Cell 1        Cell 2
            │      ▲             ▲
            │      │             │
            ├──────┼─────────────┼───────┐
            │      │             │       │
            │ ┌────┴───────┬─────┴─────┐ │
            │ │            │           │ │
    Table ◄─┼─┤ ┌────────┐ │ ┌───────┐ │ │
      Row ◄─┼─┤ └───┼────┘ │ └───┼───┘ │ │
            │ │     │      │     │     │ │
            │ └─────┼──────┴─────┼─────┘ │
            │       │            │       │
            │       ▼            ▼       │
            │    Image 1      Image 2    │
            │                            │
            │                            │
            │                            │
            │                            │
            │                            │
            │                            │
            └────────────────────────────┘
### Image Size
- Use 900px width x 300px height in order to fill two images like following screen shot
- You can play with height but avoid playing with the width in order to prevent large file size or image quality reduction

<img width="389" alt="image" src="https://user-images.githubusercontent.com/6186848/172251117-527617a1-7011-4cdc-aa20-f36e38943838.png">


### Usage
Create a new row with the following properties:
- type: 'TWO_IMAGES'
- value: ['left image ulr', 'right image ulr']



# TWO_TEXTS

### Examples of firstColumnWidth
- firstColumnWidth = 200:
<img width="682" alt="image" src="https://user-images.githubusercontent.com/6186848/172263457-c34e05ee-ec3a-4168-be3e-f16d0d156447.png">

- firstColumnWidth = 'auto':
<img width="682" alt="image" src="https://user-images.githubusercontent.com/6186848/172263485-9407d95c-055b-4641-86ee-c9eb2ec64ce0.png">

# TEXT_IMAGE
### Example
- value: ['lorem ipsum', '900x400.png'] textMargin: [0, 32], fontSize: 12, alignament: 'center'
<img width="741" alt="image" src="https://user-images.githubusercontent.com/6186848/172305064-58193f71-a1d8-4660-8d3a-fccd8846b65b.png">

- value: ['{GIFTCARD_CODE_IMAGE}', '900x400.png'], textMargin: [0, 32], barcodeWidth: 180
<img width="741" alt="image" src="https://user-images.githubusercontent.com/6186848/172304437-44fd04ad-f9c4-4e49-8c98-ee3969ed1eb7.png">



# Other Examples
- type: 'TEXT', value: '{GIFTCARD_CODE_IMAGE}', margin: [160, 0]
<img width="712" alt="image" src="https://user-images.githubusercontent.com/6186848/172304108-db0ff9b0-07e1-465b-bb28-7d0d37b5fe03.png">

- type: 'TEXT', value: '{GIFTCARD_CODE_IMAGE}', margin: [168, 16, 0, 0]
- type: 'TEXT', valie: '{GIFTCARD_CODE_TEXT}', alignment: 'center'
<img width="741" alt="image" src="https://user-images.githubusercontent.com/6186848/172308392-83e953c2-6a18-4be0-a317-40a0fc2f82c5.png">
