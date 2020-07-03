# Device not found on port, board is continuously resetting

There are different possible reasons why your board is not shown in the Arduino IDE ports tab.

If you run into this problem make the following checks before contacting Arduino Technical Support.

1. All the MKR boards with headers are shipped with a foam. This foam is slightly conductive for protecting the board from ESD during shipping, if you keep it on the pins when you attempt to use the board it can cause interference between pins and cause unwanted resets.

2. If the protective foam has been removed, then check that the latest version of the core has been installed correctly for your board: To do this simply go to Arduino IDE > Tools > Board > Boards Manager. In the pop-up window search for the name and model of your board. The right core will show in the results, then simply click 'Install' or 'Update' accordingly.
