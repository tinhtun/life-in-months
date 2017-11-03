# life-in-months
Visualizing your life expctancy in months

## Initial sketch
``` html
<div id="resultsTable">
    <table id='summaryOfResults' border='1'>
        <tbody id="body">
            
        </tbody>
    </table>
</div>
<div id="tableButtons">
    <button id='copyButton' onclick=''>Copy Table</button>
    <button id='clear' onclick='clearTable();'>Clear Table</button>
    <button id='write' onclick='writeTable();'>Write Table</button>
</div>
```

``` javascript
var rows = 30;
var columns = 36;

function writeTable() {
    var tbody = $('#body');
    for (var i = 0; i < rows; i++) {
        var tr = $('<tr/>').appendTo(tbody);
        for (var j = 0; j < columns; j++) {
            tr.append('<td>' + (i + j) + '</td>');
        }
    }
}
```
