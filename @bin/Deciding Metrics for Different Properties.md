## For `nav` menus

|**Property**|**Recommended Unit**|**Reason**|
|---|---|---|
|`font-size`|`rem`|Keeps consistent with site-wide typography|
|`padding` (inside)|`em`|Scales with text size of the link (button-like behavior)|
|`margin` (between)|`rem`|Keeps spacing uniform between links|
|`gap` (if flex)|`rem`|Consistent layout spacing|


|Unit|Based On|In Your Case|
|---|---|---|
|`rem`|Root font size (`html`)|1rem = 16px|
|`em`|**Current element’s font size**|1em = 12px (because you set font-size: 0.75rem)|