![HideUnhide.jpg](images/Hide-Unhide-Rows-And-Columns_HideUnhide.jpg "HideUnhide.jpg")

(Rows 1 and 3, and columns A and C are hidden)

```c#
var wb = new XLWorkbook();
var ws = wb.Worksheets.Add("Hide Unhide");

ws.Columns(1, 3).Hide();
ws.Rows(1, 3).Hide();

ws.Column(2).Unhide();
ws.Row(2).Unhide();

wb.SaveAs("HideUnhide.xlsx");
```
