<!-- default file list -->
*Files to look at*:

* [CustomEvents.cs](./CS/WebSite/App_Code/CustomEvents.cs) (VB: [CustomEvents.vb](./VB/WebSite/App_Code/CustomEvents.vb))
* [Helpers.cs](./CS/WebSite/App_Code/Helpers.cs) (VB: [Helpers.vb](./VB/WebSite/App_Code/Helpers.vb))
* [Default.aspx](./CS/WebSite/Default.aspx) (VB: [Default.aspx](./VB/WebSite/Default.aspx))
* [Default.aspx.cs](./CS/WebSite/Default.aspx.cs) (VB: [Default.aspx.vb](./VB/WebSite/Default.aspx.vb))
<!-- default file list end -->
# How to implement word wrapping in the resource headers


<p>To accomplish this task, it is necessary to define a table in the <strong>HorizontalResourceHeaderTemplate</strong> and apply several CSS attributes to this table as follows:</p>

```aspx
        <dxwschs:ASPxScheduler ID="ASPxScheduler1" runat="server" ...>
            <Templates>
                <HorizontalResourceHeaderTemplate>
                    <table style="margin: 0px auto;">
                        <tr>
                            <td style="padding: 2px; word-wrap: break-word; white-space: normal;">
                                <%# Container.Resource.Caption %>
                            </td>
                        </tr>
                    </table>
                </HorizontalResourceHeaderTemplate>
            </Templates>
        </dxwschs:ASPxScheduler>
```

<p> </p><p><strong>See </strong><strong>A</strong><strong>lso:</strong><br />
<a href="http://demos.devexpress.com/ASPxSchedulerDemos/Templates/ResourceHeaderTemplate.aspx"><u>Templates - Resource Headers</u></a><br />
</p>

<br/>


