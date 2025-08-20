# WinForms Spreadsheet - Sorting and Filtering the records

This sample illustrates about enabling the Sorting and Filtering feature in [WinForms Spreadsheet](https://www.syncfusion.com/winforms-ui-controls/spreadsheet).

By default, the `Spreadsheet` does not allow filtering support, so if you want to enable filtering in `Spreadsheet`, set the [AllowFiltering](https://help.syncfusion.com/cr/wpf/Syncfusion.UI.Xaml.Spreadsheet.SfSpreadsheet.html#Syncfusion_UI_Xaml_Spreadsheet_SfSpreadsheet_AllowFiltering) property to be `true`.

``` csharp
spreadsheet.AllowFiltering = true;
```

### Limitations

#### Sorting

* Sorting label in Microsoft Excel should be varied in filter popup depending on the value type in a column (for example, “Sort Smallest to Largest” for numerical values, “Sort A to Z” for string values, etc.). But sort label is not varied in `Spreadsheet` based on values due to improving filter popup loading efficiency.

* If the column is sorted in Microsoft Excel, Sort Ascending or Sort Descending is not checked in the filter popup.Since XlsIO currently has no support when importing the workbook to get the sorted order.

#### Filtering

* If the filter is applied in Microsoft Excel, the filter will be cleared from all columns while clearing the filter from any column in `Spreadsheet`.