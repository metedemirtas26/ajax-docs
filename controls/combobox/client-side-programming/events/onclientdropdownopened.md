---
title: OnClientDropDownOpened
page_title: OnClientDropDownOpened | UI for ASP.NET AJAX Documentation
description: OnClientDropDownOpened
slug: combobox/client-side-programming/events/onclientdropdownopened
tags: onclientdropdownopened
published: True
position: 3
---

# OnClientDropDownOpened



## 

As of Q1 SP2, the RadComboBox exposes a new client-side event - __OnClientDropDownOpened__.

The __OnClientDropDownOpened__ client-side event occurs after the drop-down list has been opened.

The event handler receives two parameters:

1. The instance of the combobox firing the event.

1. An eventArgs parameter containing the following method:

* __get_domEvent()__ returns the DOM event object of the drop-down opened.

You can use this event to perform any client-side actions when the drop-down is completely opened:

````ASPNET
	    <script type="text/javascript">
	        function OnClientDropDownOpenedHandler(sender, eventArgs) {
	            alert("The dropdown is opened now");
	        }
	    </script>
	    <telerik:radcombobox 
	        id="RadComboBox1" 
	        onclientdropdownopened="OnClientDropDownOpenedHandler"
	        runat="server">
	    </telerik:radcombobox>
````



# See Also

 * [OnClientDropDownOpening]({%slug combobox/client-side-programming/events/onclientdropdownopening%})