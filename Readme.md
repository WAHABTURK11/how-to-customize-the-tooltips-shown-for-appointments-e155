<!-- default file list -->
*Files to look at*:

* [Form1.cs](./CS/AppointmentToolTips/Form1.cs) (VB: [Form1.vb](./VB/AppointmentToolTips/Form1.vb))
* [Program.cs](./CS/AppointmentToolTips/Program.cs) (VB: [Program.vb](./VB/AppointmentToolTips/Program.vb))
<!-- default file list end -->
# How to customize the tooltips shown for appointments


<p>Problem:</p><p>How can I control the tooltip appearance and a tooltip message which is shown for each appointment?  For instance, I want to change the font color and backcolor of every tooltip, and make them show not only the appointment's description, but also its subject and location. How can this be done?</p><p>Solution:</p><p>A SchedulerControl provides the <a href="http://documentation.devexpress.com/#WindowsForms/DevExpressXtraEditorsBaseControl_ToolTipControllertopic">TooltipController</a> property. Use it to specify the tooltip controller, which controls the appearance of the appointment tooltips. <br />
You should create a new <strong>TooltipController</strong>, assign it to the <strong>SchedulerControl.TooltipController</strong> property, and then set the values of the required properties. Also, you can handle the <a href="http://documentation.devexpress.com/#CoreLibraries/DevExpressUtilsToolTipController_BeforeShowtopic">TooltipController.BeforeShow</a> event to specify a custom text for the tooltips.<br />
The following example illustrates this approach. Check the <strong>SuperTips</strong> checkbox to display <a href="http://documentation.devexpress.com/#CoreLibraries/clsDevExpressUtilsSuperToolTiptopic">SuperToolTips</a>.</p>

<br/>


