# Excel Week 3 Wrap-Up: Formatting# Excel Week 3 Wrap-Up: Formatting

## Main Idea

Week 3 focuses on formatting Excel worksheets so they are easier to read, more professional, and more consistent.

Formatting usually does not change the data itself. It changes how the data looks so readers can understand it faster.

---

# 1. Why Formatting Matters

Good formatting makes a spreadsheet:

- easier to read
- more professional
- more visually organized
- easier to present
- more consistent across worksheets and workbooks

A spreadsheet can contain correct data, but if it is messy or hard to read, it may still be ineffective.

---

# 2. Font Tools

Most basic formatting tools are found on the **Home** tab of the ribbon, especially in the **Font** group.

Font tools include:

| Tool | Purpose |
|---|---|
| Font type | Changes the style of text |
| Font size | Makes text larger or smaller |
| Bold | Makes text stand out |
| Italics | Adds emphasis |
| Underline | Adds a line under text |
| Fill color | Changes the cell background color |
| Font color | Changes the text color |

Before applying formatting, always select the cell or range you want to change.

---

# 3. Live Preview

Excel often shows a **live preview** when you hover over formatting options.

This lets you see what the formatting will look like before applying it.

The worksheet only changes when you click the option.

---

# 4. Borders

Borders help separate data and make tables easier to read.

The **Borders** tool is in the Font group and looks like a small window.

Common border options:

| Border Option | Use |
|---|---|
| All Borders | Adds borders around every selected cell |
| Thick Outside Borders | Adds a border around the outside only |
| Top and Double Bottom Border | Useful for total rows |
| More Borders | Lets you customize line style, color, and placement |
| No Border | Removes borders |

Tip: Add borders when the spreadsheet is close to finished, because editing later can make borders harder to manage.

---

# 5. Alignment Tools

Alignment changes where data sits inside a cell.

Alignment tools are on the **Home** tab near the Font group.

## Horizontal Alignment

| Option | Meaning |
|---|---|
| Left align | Moves content to the left |
| Center align | Centers content horizontally |
| Right align | Moves content to the right |

## Vertical Alignment

| Option | Meaning |
|---|---|
| Top align | Places content at the top |
| Middle align | Centers content vertically |
| Bottom align | Places content at the bottom |

Alignment is useful for making headings and tables look cleaner.

---

# 6. Wrap Text

**Wrap Text** makes long text fit inside a cell by moving it onto multiple lines.

Use Wrap Text when:

- headings are too long
- you do not want very wide columns
- text does not fit properly in the cell

This is especially useful for column headings.

---

# 7. Merge and Center

**Merge and Center** combines selected cells into one larger cell and centers the text.

It is useful for large headings above a table.

## Warning

Use Merge and Center carefully:

- Use it mainly for headings.
- Do not use it inside data areas.
- If more than one selected cell contains data, you may lose data.
- Merged cells can cause problems when sorting and filtering.

---

# 8. Orientation

**Orientation** changes the direction or angle of text.

This is useful when headings are long but you do not want to make columns wider.

Examples:

- angle counterclockwise
- rotate text up
- rotate text down
- vertical text

---

# 9. Format Painter

**Format Painter** copies formatting from one cell or range to another.

It is located in the **Clipboard** group on the Home tab.

## Why It Is Useful

Format Painter helps you:

- save time
- copy multiple formatting choices at once
- keep formatting consistent
- avoid repeating steps manually

It can copy formatting such as bold, italics, font color, fill color, borders, number formats, and alignment.

---

# 10. Clear Formats

**Clear Formats** removes formatting but keeps the cell contents.

Do not confuse it with **Clear All**.

| Option | What It Does |
|---|---|
| Clear Formats | Removes formatting only |
| Clear All | Removes contents and formatting |

Clear Formats can also remove number formatting, so use it carefully.

---

# 11. Number Formats

Number formats change how numbers are displayed.

They do not always change the actual stored value.

Common number formats:

| Format | Purpose |
|---|---|
| General | Default format with no special display |
| Currency | Displays numbers as money |
| Accounting | Displays money with currency symbol aligned left |
| Percentage | Displays decimals as percentages |
| Short Date | Displays dates in compact form |
| Long Date | Displays dates in longer written form |

---

# 12. Currency vs Accounting

Currency and Accounting formats look similar, but they display values differently.

| Format | Difference |
|---|---|
| Currency | Currency symbol appears close to the number |
| Accounting | Currency symbol aligns to the left side of the cell |

Avoid mixing Currency and Accounting in the same dataset because it can look inconsistent.

---

# 13. Percentages

Excel stores percentages as decimals.

Example:

```excel
0.05
```

When formatted as a percentage, this displays as:

```text
5%
```

You can also type a value directly as a percentage, such as:

```text
10%
```

Excel will recognize it and apply percentage formatting.

---

# 14. Dates

Dates in Excel are stored as numbers but displayed as dates.

Excel counts dates from January 1, 1900.

This is why Excel can calculate with dates.

## Important Warning

Use date formats Excel recognizes.

If Excel does not recognize the date format, it may treat it as General data, which can cause problems with date calculations.

---

# 15. Styles

**Styles** are built-in formatting options in Excel.

They are found on the **Home** tab in the Styles gallery.

Styles help you format quickly and consistently.

Examples:

- Title
- Heading styles
- Accent styles
- Total style

Styles are useful for headings, labels, and total rows.

---

# 16. Themes

**Themes** control the overall look of a workbook.

Themes can affect:

- colors
- fonts
- styles

Themes are found on the **Page Layout** tab.

Changing a theme can update the look of the whole workbook.

---

# 17. Theme Colors and Fonts

Themes work best when you use **theme colors** and **theme fonts**.

If you manually choose non-theme colors or fonts, those cells may not update when the theme changes.

Themes can also help keep Excel, Word, and PowerPoint files visually consistent.

---

# 18. Common Mistakes to Avoid

## Mistake 1: Formatting without selecting cells first

Always select the correct cell or range before applying formatting.

## Mistake 2: Overusing borders

Too many borders can make a worksheet look cluttered.

## Mistake 3: Using Merge and Center in data areas

Merged cells can cause sorting and filtering problems.

## Mistake 4: Mixing number formats

Do not mix Currency and Accounting formats in the same dataset.

## Mistake 5: Using invalid date formats

If Excel does not recognize a date, it may not calculate correctly.

## Mistake 6: Clearing formats carelessly

Clear Formats removes number formatting too, including currency, dates, and percentages.

## Mistake 7: Ignoring theme colors and fonts

Using non-theme formatting can prevent workbook-wide theme changes from working properly.

---

# 19. Week 3 Quick Reference

| Tool | Main Use |
|---|---|
| Font tools | Change text appearance |
| Fill color | Change cell background |
| Font color | Change text color |
| Borders | Separate data visually |
| Alignment | Position data inside cells |
| Wrap Text | Fit long text inside cells |
| Merge and Center | Create centered headings |
| Orientation | Rotate or angle text |
| Format Painter | Copy formatting quickly |
| Clear Formats | Remove formatting |
| Number formats | Display numbers correctly |
| Styles | Apply consistent built-in formatting |
| Themes | Change workbook-wide colors and fonts |

---

# Big Lesson

Formatting is not just decoration.

Good formatting makes data easier to understand, improves readability, and helps create professional, consistent worksheets.

---

# Final Summary

Week 3 focuses on formatting Excel worksheets. Font tools help adjust text, colors, and cell backgrounds. Borders organize tables visually, while alignment tools position data inside cells. Wrap Text helps long text fit, Merge and Center is useful for headings, and Orientation can rotate text to save space. Format Painter quickly copies formatting, while Clear Formats removes unwanted formatting. Number formats display values as currency, accounting, percentages, or dates. Styles and Themes help keep formatting consistent across worksheets and workbooks. The main lesson is that formatting should make data clearer, more readable, and more professional.

## Main Idea

Week 3 focuses on formatting Excel worksheets so they are easier to read, more professional, and more consistent.

Formatting does not usually change the actual data. Instead, it changes how the data looks.

Good formatting helps people understand a spreadsheet faster.

---

# 1. Why Formatting Matters

Formatting is important because it makes a worksheet:

- easier to read
- more professional
- more visually organized
- easier to present to others
- more consistent across worksheets and workbooks

A spreadsheet may contain correct data, but if it is difficult to read, it can still be ineffective.

---

# 2. Font Tools

Most basic formatting tools are found on the Home tab of the ribbon.

The Font group includes tools for changing:

- font type
- font size
- bold
- italics
- underline
- fill color
- font color

---

# 3. Selecting Cells Before Formatting

Before applying formatting, you must select the cell or cells you want to change.

You can select:

- one cell
- a range of cells
- an entire row
- an entire column
- a whole worksheet area

Excel applies the formatting only to the selected area.

---

# 4. Font Type

The font controls the style of the text.

Excel’s default font is usually Calibri, which is readable and simple.

When choosing fonts, it is usually best to follow the organization’s standard fonts.

---

# 5. Live Preview

When you hover over font options, Excel may show a live preview.

This lets you see what the formatting will look like before applying it.

The worksheet does not actually change until you click the option.

---

# 6. Font Size

Font size controls how large or small text appears.

Increasing the font size is useful for:

- titles
- headings
- section labels
- important values

Decreasing font size can help fit text into cells, but it should not make the worksheet hard to read.

---

# 7. Increase Font and Decrease Font

Excel has quick buttons to increase or decrease font size.

These are useful for small adjustments without choosing an exact font size from the dropdown.

---

# 8. Bold, Italics, and Underline

These tools work like on/off switches.

Click once to apply.

Click again to remove.

## Bold

Bold makes text stand out.

Useful for:

- headings
- totals
- important labels

## Italics

Italics can emphasize text.

Useful for:

- notes
- secondary labels
- special comments

## Underline

Underline adds a line under text.

Useful for headings, but should be used carefully so the sheet does not look cluttered.

---

# 9. Fill Color and Font Color

Excel has two important color tools:

| Tool | Purpose |
|---|---|
| Fill color | Changes the background color of the cell |
| Font color | Changes the color of the text |

Example:

A dark blue fill with white font can make headings stand out clearly.

---

# 10. Borders

Borders help separate and organize data visually.

The Borders tool is located in the Font group.

The icon looks like a small window.

---

# 11. Applying Borders

Before applying borders, select the cells where you want borders.

Common border options include:

- All Borders
- No Border
- Thick Outside Borders
- Top and Double Bottom Border
- More Borders

---

# 12. All Borders

All Borders adds borders around every selected cell.

This can make a table easier to read because each cell is clearly separated.

---

# 13. Top and Double Bottom Border

This option is useful for total rows.

It applies:

- a line at the top
- a double line at the bottom

This helps the total row stand out from the rest of the data.

---

# 14. Thick Outside Borders

Thick Outside Borders adds a border only around the outside of the selected range.

It does not add lines between the cells.

This is useful when you want to frame a table or section without making every cell look boxed in.

---

# 15. More Borders

More Borders opens a dialog box where you can customize borders.

You can change:

- line style
- line thickness
- border color
- border placement

You can choose exactly where the border should appear, such as only on the bottom of selected cells.

---

# 16. Removing Borders

To remove borders:

1. Select the cell or range.
2. Open the Borders dropdown.
3. Choose No Border.

Be careful: removing a border from one cell may also affect a neighboring cell if they share the same border.

---

# 17. Border Tip

It is usually best to wait until the spreadsheet is close to finished before adding many borders.

If you add borders too early, later editing may make the formatting harder to manage.

---

# 18. Alignment Tools

Alignment tools change the position of data inside a cell.

They are located on the Home tab, near the Font group.

Alignment can be:

- horizontal
- vertical

---

# 19. Horizontal Alignment

Horizontal alignment controls whether content sits on the left, center, or right of a cell.

Common options:

| Alignment | Meaning |
|---|---|
| Left align | Content moves to the left |
| Center align | Content is centered horizontally |
| Right align | Content moves to the right |

---

# 20. Vertical Alignment

Vertical alignment controls whether content sits at the top, middle, or bottom of a cell.

Common options:

| Alignment | Meaning |
|---|---|
| Top align | Content sits at the top |
| Middle align | Content sits vertically centered |
| Bottom align | Content sits at the bottom |

Vertical alignment is especially useful when row height is larger than normal.

---

# 21. Wrap Text

Wrap Text makes long text fit inside a cell by moving it onto multiple lines.

This is useful when:

- headings are too wide
- column names are long
- you do not want to make columns wider

Wrap Text can make headings easier to read without expanding the worksheet too much.

---

# 22. Merge and Center

Merge and Center combines multiple selected cells into one larger cell and centers the text.

This is useful for large headings that need to sit above a table.

---

# 23. Merge and Center Warning

Use Merge and Center carefully.

Important warnings:

- Only use it when there is text in one of the selected cells.
- If multiple selected cells contain data, you may lose data.
- Use it mainly for headings.
- Avoid using it inside data areas.

Merged cells can cause problems later when sorting and filtering data.

---

# 24. Orientation

Orientation changes the angle or direction of text in a cell.

This is useful when column headings are long but you do not want wide columns.

Examples of orientation options:

- angle counterclockwise
- rotate text up
- rotate text down
- vertical text

This can make headings fit better in narrow columns.

---

# 25. Format Painter

The Format Painter copies formatting from one cell or range to another.

It is located in the Clipboard group on the Home tab.

---

# 26. Why Format Painter Is Useful

Format Painter helps you:

- save time
- copy multiple formatting choices at once
- keep formatting consistent
- avoid repeating the same formatting steps manually

---

# 27. How to Use Format Painter

Basic steps:

1. Select the cell with the formatting you want to copy.
2. Click Format Painter.
3. Select the cell or range where you want to apply the formatting.

The formatting is copied, but the cell contents are not copied.

---

# 28. Copying Multiple Formats

Format Painter can copy several formatting choices at once.

For example, it can copy:

- bold
- italics
- font color
- fill color
- borders
- number formats
- alignment

This is faster than applying each formatting tool one by one.

---

# 29. Format Painter Across Worksheets

Format Painter can also copy formatting from one worksheet to another.

Example:

If the 2016 sales sheet is formatted and the 2015 sales sheet is not, you can copy the formatting from the 2016 sheet to the 2015 sheet.

This helps make worksheets consistent.

---

# 30. Clear Formats

Clear Formats removes formatting without deleting the cell contents.

It is found under the Clear tool on the right side of the ribbon.

---

# 31. Clear All vs Clear Formats

| Option | What It Does |
|---|---|
| Clear All | Removes contents and formatting |
| Clear Formats | Removes only formatting |

Use Clear Formats when you want to keep the data but remove the appearance settings.

---

# 32. Number Formats

Number formats change how numbers are displayed.

They do not necessarily change the actual stored value.

Number formatting helps numbers appear in the correct form.

Examples:

- currency
- accounting
- percentage
- short date
- long date
- general

---

# 33. General Format

When you type a number into a cell, Excel usually applies the General format by default.

General means no specific number format has been applied.

---

# 34. Currency Format

Currency format displays numbers as money.

Excel uses the currency symbol from your regional settings.

It also applies an appropriate number of decimal places.

Example:

A value may display as money instead of a plain number.

---

# 35. Accounting Format

Accounting format is similar to Currency format, but it aligns the currency symbol on the left side of the cell and adds spacing.

This makes financial statements easier to read.

---

# 36. Currency vs Accounting

| Format | Main Difference |
|---|---|
| Currency | Currency symbol appears close to the number |
| Accounting | Currency symbol aligns to the left of the cell |

It is best not to mix Currency and Accounting formats in the same dataset because it can look inconsistent.

---

# 37. Percentage Format

Percentage format displays decimal values as percentages.

Example:

If a cell contains 0.05 and you apply Percentage format, Excel displays it as 5%.

You can also type a value directly as a percentage, such as 10%.

Excel will recognize it and apply the percentage format.

---

# 38. Date Format

Dates in Excel are stored as numbers but formatted to look like dates.

Excel counts dates from January 1, 1900.

For example, the number 1 can be formatted as January 1, 1900.

---

# 39. Why Dates Are Numbers

Because dates are stored as numbers, Excel can perform calculations with dates.

This allows you to calculate things like:

- days between dates
- due dates
- timelines
- date differences

---

# 40. Valid Date Formats

Excel only recognizes certain date formats.

If you type a date in a format Excel does not recognize, it may remain as General text or a general value.

This can cause problems because Excel may not be able to calculate with it as a date.

---

# 41. Short Date and Long Date

Excel provides built-in date formats.

| Format | Example Use |
|---|---|
| Short Date | Compact date display |
| Long Date | Full written date display |

The exact appearance depends on regional settings.

---

# 42. Number Format Warning

If a cell was previously formatted as a date, then later you type a number into it, Excel may display that number as a date.

This happens because the cell still has date formatting.

To fix it, change the cell format back to General.

---

# 43. Clear Formats Warning

Clear Formats removes all formatting, including number formatting.

This means it can remove:

- font formatting
- fill color
- alignment
- borders
- currency formatting
- percentage formatting
- date formatting

Use Clear Formats carefully.

---

# 44. Styles

Styles are built-in formatting options in Excel.

They help quickly apply consistent formatting.

Styles are located on the Home tab of the ribbon in the Styles gallery.

---

# 45. Why Styles Are Useful

Styles help you:

- format quickly
- make worksheets look professional
- guarantee consistency
- reuse the same formatting across workbooks

---

# 46. Examples of Styles

Excel includes styles such as:

- Title
- Heading styles
- Accent styles
- Total
- themed cell styles

These are useful for headings, data labels, and total rows.

---

# 47. Accent Styles

Accent styles use theme colors.

Excel usually provides several accent colors.

Some accents can be applied at full strength or in lighter versions, such as 80% white.

---

# 48. Themes

Themes control the overall look and feel of a workbook.

Themes can affect:

- colors
- fonts
- styles
- workbook appearance

Themes are found on the Page Layout tab.

---

# 49. Office Theme

The Office theme is the default theme.

This is why Excel often starts with the same default font and colors.

---

# 50. Why Themes Are Powerful

Themes allow you to quickly change the styling throughout an entire workbook.

If a workbook uses theme colors and theme fonts, changing the theme updates the workbook consistently.

---

# 51. Theme Colors and Theme Fonts

Theme colors and theme fonts are connected to the selected workbook theme.

If you use non-theme colors or non-theme fonts, those cells may not update when the theme changes.

---

# 52. Important Theme Rule

To get the full benefit of themes, use theme colors and theme fonts.

If you manually choose a non-theme color or non-theme font, Excel may not update that cell when you change the theme.

---

# 53. Custom Themes

Excel allows you to mix and match:

- theme colors
- theme fonts
- full themes

You can also create custom colors and custom fonts.

However, Excel already provides many built-in options.

---

# 54. Themes Across Office

Themes exist across Microsoft Office.

This means you can create a consistent look across:

- Excel
- Word
- PowerPoint

This is helpful when creating professional reports, documents, and presentations.

---

# 55. Formatting Best Practices

Good spreadsheet formatting should be:

- consistent
- readable
- professional
- not too busy
- useful for understanding the data

Formatting should support the data, not distract from it.

---

# 56. Common Mistakes to Avoid

## Mistake 1: Formatting Before Selecting Cells

Always select the cells first.

If you do not select the correct range, formatting may be applied to the wrong cells.

---

## Mistake 2: Overusing Borders

Too many borders can make a worksheet look cluttered.

Use borders to guide the reader, not to decorate every part of the sheet.

---

## Mistake 3: Using Merge and Center Inside Data

Merged cells can cause problems when sorting and filtering.

Use Merge and Center mainly for headings.

---

## Mistake 4: Mixing Currency and Accounting Formats

Currency and Accounting formats look similar but align differently.

Mixing them in the same dataset can make the worksheet look inconsistent.

---

## Mistake 5: Using Unrecognized Date Formats

If Excel does not recognize a date format, it may not treat the value as a date.

This can prevent date calculations from working correctly.

---

## Mistake 6: Clearing Formats Without Thinking

Clear Formats removes number formatting too.

This can accidentally remove currency, percentage, or date formats.

---

## Mistake 7: Using Non-Theme Colors and Fonts

If you use non-theme colors or fonts, your workbook may not update properly when you change themes.

Use theme colors and theme fonts for better consistency.

---

# 57. Week 3 Quick Reference

| Tool | Purpose |
|---|---|
| Font type | Changes the style of text |
| Font size | Changes text size |
| Bold | Makes text stand out |
| Italics | Emphasizes text |
| Underline | Adds a line under text |
| Fill color | Changes cell background color |
| Font color | Changes text color |
| Borders | Adds lines around cells |
| Alignment | Changes position of content inside cells |
| Wrap Text | Makes long text fit inside cells |
| Merge and Center | Combines cells and centers text |
| Orientation | Rotates or angles text |
| Format Painter | Copies formatting |
| Clear Formats | Removes formatting |
| Number formats | Changes how numbers appear |
| Styles | Applies built-in formatting quickly |
| Themes | Controls workbook-wide fonts and colors |

---

# 58. Big Lesson

Formatting is not just about making a spreadsheet look nice.

It helps make data easier to understand.

The best formatting is consistent, readable, and purposeful.

---

# Final Summary

Week 3 focuses on formatting Excel worksheets to make them more readable, professional, and consistent. Font tools help change text appearance with font type, font size, bold, italics, underline, fill color, and font color. Borders help separate and organize data visually. Alignment tools control how content sits inside cells, while Wrap Text, Merge and Center, and Orientation help manage headings and long text. Format Painter copies formatting quickly, and Clear Formats removes unwanted formatting. Number formats control how values appear as currency, accounting, percentages, and dates. Styles provide built-in formatting options, while Themes allow workbook-wide control of colors and fonts. The main lesson is that good formatting helps readers understand data faster and keeps worksheets consistent across a workbook.
