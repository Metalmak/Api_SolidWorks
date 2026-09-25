<!-- source: sldworksapiprogguide/Overview/Sorting_Tables.htm -->

# SOLIDWORKS API Help

# Sorting Tables

### To sort and re-sort a Bill of Materials (BOM) table:

1. Select a BOM table annotation in
   the graphics area.
2. Call
   ISelectionMgr::GetSelectedObject6
   to get the selected
   ITableAnnotation.
3. Cast the selected
   ITableAnnotation
   object to an
   IBomTableAnnotation.
4. Call
   IBomTableAnnotation::GetBomTableSortData to create an
   IBomTableSortData object.
5. Set the properties of
   IBomTableSortData to define the sort.
6. (Optional) Set
   IBomTableSortData::SaveCurrentSortParameters to true to save the sort
   settings to the BOM table in the document during the sort. This allows you
   to re-sort the table at a later date. See step 8.
7. Sort the table by calling
   IBomTableAnnotation::Sort,
   passing the
   IBomTableSortData
   object in SortData.
8. To re-sort the table at a later date, you can perform steps 1-7. But if
   you previously performed steps 6 and 7 to save the sort settings to the BOM
   table, you can quickly re-sort the table by only performing steps 1-4 and
   calling
   IBomTableAnnotation::ApplySavedSortScheme, which applies the sort
   settings saved in the BOM table.

### To sort a hole table:

1. Select a hole table
   annotation in the graphics area.
2. Call
   ISelectionMgr::GetSelectedObject6
   to get the selected
   ITableAnnotation.
3. Cast the selected
   ITableAnnotation
   object to an
   IHoleTableAnnotation.
4. Because hole tables must be sorted on the Tag column, call
   IHoleTableAnnotation::Sort(ColumnIndex, SortAscending), where
   ColumnIndex = 0 and SortAscending = true for an ascending sort.

### To sort a general table:

1. Select a general table annotation
   in the graphics area.
2. Call
   ISelectionMgr::GetSelectedObject6
   to get the selected
   ITableAnnotation.
3. Cast the selected
   ITableAnnotation
   object to an
   IGeneralTableAnnotation.
4. Call
   IGeneralTableAnnotation::Sort.

### To sort a weldment cut list table:

1. Select a weldment cut list table annotation in the
   graphics area.
2. Call
   ISelectionMgr::GetSelectedObject6
   to get the selected
   ITableAnnotation.
3. Cast the selected
   ITableAnnotation
   object to an
   IWeldmentCutListAnnotation.
4. Because weldment cut list tables must be sorted on any
   column except Item Number, call
   IWeldmentCutListAnnotation::Sort(ColumnIndex, SortAscending), where
   ColumnIndex > 0 and SortAscending = true for an ascending sort.