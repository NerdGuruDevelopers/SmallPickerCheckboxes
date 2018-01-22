# SmallPickerCheckboxes
A CSS snippet for creating custom small checkboxes for things like days, months, minutes and seconds.

I wanted a small snipet of code which would allow me to create custom checkboxes on the fly. Ideally one that would work well with for loops and date time selections. Supports strings up to 3 characters currently. Here are some examples of what you can do with this CSS:

<div align="center">
    <img src="http://nerd.guru/screenshots/chrome_2018-01-22_09-10-41.png" />
</div>

<hr>

<div align="center">
    <img src="http://nerd.guru/screenshots/chrome_2018-01-22_09-11-13.png" />
</div>

<hr>

<div align="center">
    <img src="http://nerd.guru/screenshots/chrome_2018-01-22_09-11-38.png" />
</div>

<hr>

HTML (With Smarty) Usage Example:

    {foreach ["S", "M", "T", "W", "T", "F", "S"] as $day}
        <span class="icheck_wrapper">
            <input type="checkbox" class="icheck" value="{$day}" data-value="{$day}" data-width="{strlen($day)}" name="days[]" checked="checked" />
        </span>
    {/foreach}

Output:

Prints out 7 custom checkboxes, one for each day of the week. Each is selectable or deselectable by the user.

<div align="center">
<img src="http://nerd.guru/screenshots/chrome_2018-01-22_09-10-41.png" />
</div>
