# Osmanli Calendar

Osmanli Calendar is a jQuery plug-in for generating professional date pickers and calender. it is easy to use.

## Installation

Use [npm](https://www.npmjs.com/package/osmanli-calender) to install Osmanli Calendar.

```bash
npm i osmanli-calender
```

## Example
Html Code:
```html
<div>
<span class="month-year"></span>
<table class="date_table">
<tr>
<th>S</th> <th>M</th> <th>T</th><th>W</th>
<th>T</th> <th>F</th> <th>S</th>
</tr>
</table>
<span class="prev-month">Previous</span>
<span class="next-month">next</span>
</div>
```
JavaScript Code:
```javascript
var start_date_dialog = osmanli_calendar
$('.prev-month').click(function () {start_date_dialog.pre_month()});
$('.next-month').click(function () {start_date_dialog.next_month()});
  
start_date_dialog.ON_SELECT_FUNC = onDateSelect_from
start_date_dialog.init()
```
## Options
Method/Options | Usage
------------ | -------------
`CURRENT_DATE` (var) | `osmanli_calendar.CURRENT_DATE` is used to specify the starting date
`SELECT_DATE` (var) | `osmanli_calendar.SELECT_DATE` is used to specify the selected date
`DAYS_DISABLE_MIN`/`DAYS_DISABLE_MIN` (var) | `osmanli_calendar.DAYS_DISABLE_MIN` and `osmanli_calendar.DAYS_DISABLE_MAX`used to specify if to disable dates between certain limit. Default value: `OFF` Enable State: `On`
`MAX_DATE`/`MIN_DATE` (var) | `osmanli_calendar.MIN_DATE` and `osmanli_calendar.MAX_DATE` are used to set the limiting date. Accepted values are always `Date()` objects.
`ON_SELECT_FUNC` (function) | `osmanli_calendar.ON_SELECT_FUNC` is the callback function when a date is selected.

## Acknowledgment
Dedicated to Sheykh Lokman Effendi Hz, who is always blessing me with the countless blessing and divine favors.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update the tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
