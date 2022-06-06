# TWO_IMAGES
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
