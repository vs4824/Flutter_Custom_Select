# Flutter Custom Select

FLutter Custom Selector is a package for creating single-select as well ass multi-select widgets with an awesome and unique user interface.

## Features

1. Supports FormField features like validator.

2. Awesome default design.

3. BottomSheet widget.

4. Make your multi selection awesome.

5. All selection field is enabled in multi selection field.

## Usage

### CustomSingleSelectField

This widget provide an GestureDetector which open the bottom sheet and are equipped with FormField features. You can customize it using the provided parameters.

To store the selected values, you can use the onSelectionDone parameter.

   ```
   CustomSingleSelectField<String>(
  items: dataString,
  title: "Country",
  onSelectionDone: (value){
    selectedString = value;
    setState(() {});
  },
  itemAsString: (item)=>item,
),
   ```

### CustomMultiSelectField

This widget provide an GestureDetector which open the bottom sheet and are equipped with FormField features. You can customize it using the provided parameters.

To store the selected values, you can use the onSelectionDone parameter.

   ```
   CustomMultiSelectField<String>(
  title: "Country",
  items: dataString, 
  enableAllOptionSelect: true,
  onSelectionDone: _onCountriesSelectionComplete,
  itemAsString: (item) => item.toString(),
),
   ```
