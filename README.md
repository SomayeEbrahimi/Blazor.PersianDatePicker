# PersianDatePicker

<img src="https://github.com/fericode/blazor-jalali-datepicker/blob/main/screenshot.png">

## Usage:

1- Install **Blazor.PersianDatePicker** from Nuget

2- Add `<script src="_content/Blazor.PersianDatePicker/datepicker.min.js" type="text/javascript"></script>` to your **index.html** or **_Host.cshtml**

3- Add `<link href="_content/Blazor.PersianDatePicker/datepicker.css" rel="stylesheet" />` to your **index.html** or **_Host.cshtml**

4- Add `@using Blazor.PersianDatePicker` to **_imports.razor**

5- Use the component :)


```
<InputPersianDatePicker 
                        // Html input element id attribute 
                        Id="myInputDatePicker" //Required 

                        // Bind input value to local variable or dto etc
                        @bind-Value="_myComponentField"

                        // Html input element name attribute
                        Name="myInputName" //Optional

                        // Control visibility of input
                        Visible="true" //Default: true

                        // ReadOnly make input disabled. Meaning only showing value and picker popup won't open
                        ReadOnly="false" //Default: false

                        // Picker align relative to input
                        // Options: Align.Right | Align.Left
                        PickerAlign="Align.Right" //Default: Align.Right

                        // Can be used in changing vertical position of picker popup relative to input
                        PickerOffsetTopPositionInPixels="2" //Default: 2

                        // Initial value for input set on today
                        InitialValue="false" //Default: false

                        // Calendar type for date picker including Dual, Single, etc
                        // Options: Calendar.DualModeJalaliDefault | Calendar.DualModeMiladiDefault | Calendar.SingleModeJalali | Calendar.SingleModeMiladi
                        CalendarType="Calendar.DualModeJalaliDefault" //Default: Calendar.DualModeJalaliDefault

                        // Control the digit type showing in input after selecting by picker
                        // Options: DigitType.BasedOnCalendar | DigitType.Persian | DigitType.Persian
                        DigitType="DigitType.BasedOnCalendar" //Default: DigitType.BasedOnCalendar

                        // Format of date to show in input after selecting by picker, e.g. 1400/01/01 or 1400-01-01
                        // Options: DateFormat.yyyy_slash_MM_slash_dd | DateFormat.yyyy_dash_MM_dash_dd
                        DateFormat="DateFormat.yyyy_slash_MM_slash_dd" //Default: DateFormat.yyyy_slash_MM_slash_dd

                        // Prevent user select date before today
                        MinDateSetOnToday="true" //Default: true

                        // Input placeholder
                        Placeholder="Select date"

                        // CSS class for input element
                        CssClass="form-control"

                        // Inline styles for input element
                        Style="border:1px solid red; width:50%"

                        // Choose a theme for changing look and feel of picker
                        Theme="PickerTheme.Default"

                        // Input onchange event
                        OnChange="@(() => Console.WriteLine("OK"))" />

```

## Performance:

   * **js size: 33 KB** => gzipped (IIS server uses compressed gzip files out of the box (as default) for Blazor Web Assembly Hosted applications. For Blazor Standalone app, though, some manual steps is required)

   * **css size: 3 KB** => gzipped

   * **dll size: 14 KB**
